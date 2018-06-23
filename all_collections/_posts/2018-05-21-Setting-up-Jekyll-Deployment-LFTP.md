---

title: Setting up automatic Jekyll deployment with LFTP and Bash. 
date: 2018-05-22T17:01:27+00:00
permalink: /jekyll-automatic-deployment-ftp/
header:
  teaser: /assets/images/uploads/2018/05/jeykll_and_ftp.jpg
classes: wide
image:
  path: /assets/images/uploads/2018/05/jeykll_and_ftp.jpg
categories:
  - programming
tags:
  - Jekyll
  - Automation
  - 
---
Jekyll is the most popular static site generator which brings the benefit of avoiding a database totally.
Recently, I migrated from wordpress to jekyll and found the deployment process to be repetitive.The best way to deploy it on a FTP server is to use LFTP which can be installed by following command on a debian OS.
`apt-get install lftp`

 LFTP is a CLI based ftp client with extensive list of configurations.  You need to use reverse mirror mode to mirror files from localhost to server.

![Working of lftp](/assets/images/uploads/2018/05/working-LFTP-reverse-mode.png){: .align-center}

Next step is to create a bash script. 

```
#!/bin/bash

# Local - Blog directory
JEKYLL_LOCAL_DIRECTORY="/home/username/codehealthy-deploy/"
JEKYLL_DIRECTORY="/home/username/codehealthy/"
SERVER_DIRECTORY="/public_html/"
JEKYLL_CONFIG_FILE="_config.yml"
#!/bin/bash

file='deploydetails.txt'
if [ -f "$file" ];then
 source $file
else
  echo "Ftp details file not found. Please create ${file} with details\nhostname\nusername\npassword"
  exit
fi
###################################
#DRY_RUN="--dry-run"               #
READ_WARNING=1

  if [ -z "$password" ]; then
 echo "Password is not set. Exiting. Please set password in ${file}"

 exit
fi
   if [ -n "$DRY_RUN" ]; then
 echo "Don' worry. Dry run is on. The Script won't actually delete file"
 else
   echo "The Script WILL Actually Delete Files......"

fi

if [ -n "$READ_WARNING" ]; then
  echo "#############################################################"
 echo "Warning::"
 echo " You acknowledge that Running the script might delete files. "
  echo "Comment \"READ_WARNING=1\" to hide warning"
    echo "#############################################################"
    exit

fi  

do_work() {

if [ -d "$JEKYLL_LOCAL_DIRECTORY" ]; then

  # kill existing jekyll process
  pkill jekyll 
 
  # wait for a while
  sleep 5

  cd ${JEKYLL_DIRECTORY}
 JEKYLL_ENV=production bundle exec jekyll build --source ${JEKYLL_DIRECTORY} --destination ${JEKYLL_LOCAL_DIRECTORY} --config ${JEKYLL_CONFIG_FILE} || return 1
  
  lftp -u ${username},${password} -e "mirror -R -p -P=10 --exclude sensitiveFolder/ --only-newer --ignore-time -vvv  $DRY_RUN ${JEKYLL_LOCAL_DIRECTORY}/ ${SERVER_DIRECTORY};quit" ftp://${hostname} || return 1
fi
  
return 0
}

report() {
 
  ##zenity --info --title "Jekyll deployment" --text "All done. Hurray" --timeout=10  #Popup
  [ "$1" = "ok" ]&& notify-send "Jekyll Deployment" "Successfuly Completed" 2>/dev/null && echo "done"
  [ "$1" != "ok" ] && notify-send "Jekyll Deployment" "Error occured." 2>/dev/null && echo "error"
  return 0
}

do_work && report ok || report err
```

Finally, You need to create a file named `deploydetails.txt` in the folder where you created your `bash script` having following information.

```
hostname="yourhost.com"
username='yourUsernameHere'
password='yourPasswordHere'
#please enclose your password and username in single quotes
```



## Don't forget to exclude all files and directories such as addon domains directories, sensitive data from mirroring. 
{: .notice--danger}

For example, If you want to exclude a folder named `sensitiveFolder`, you need to pass `--exclude sensitiveFolder/`

You can chain the command `--exclude sensitiveFolder/ --exclude sensitiveFolder2/ --exclude sensitiveFolder/3` to exclude multiple folders.


Also, LFTP provides regex pattern matching for exluding or including folders.

Lastly, the script provides a notification on its completion.

