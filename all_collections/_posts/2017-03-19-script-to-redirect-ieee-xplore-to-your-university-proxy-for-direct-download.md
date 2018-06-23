---
id: 2342
title: Script to redirect IEEE xplore to Your University Proxy for direct download
date: 2017-03-19T03:23:21+00:00
permalink: /script-to-redirect-ieee-xplore-to-your-university-proxy-for-direct-download/
header:
  teaser: /assets/images/uploads/2017/03/click-add-arrow.png
categories:
  - google-chrome
---
This script is for those who want to access IEEE xplore from their home but need to log in every time.
  
So this script redirects every web page that has
  
`http://ieeexplore.ieee.org/document/7880546/` 
  
to University page.
  
`http://ieeexplore.ieee.org.proxy.library.carleton.ca/stamp/stamp.jsp?arnumber=`
  
For example, in this case, it redirects to direct download through the proxy of Carleton University.

You need to download <a href="https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo?hl=en" target="_blank">tampermonkey</a>
  
Then click plus icon and paste the following script.
![screenshot](/assets/images/uploads/2017/03/click-add-arrow.png)

{% gist d748a512d41ac1c66e94e9fe8e8682a8 %}