---
title: AutohotKey Script Tutorial to AutoUpdate Boxifier Software
date: 2017-01-07T01:13:06+00:00
permalink: /autohotkey-script-tutorial-to-autoupdate-boxifier-software/
header:
  teaser: /assets/images/uploads/2017/01/boxifier-update.jpg
categories:
  - AutoHotKey
---
Boxifier is a software that allows you to selective sync folder with dropbox from any drive on your computer.<img class="alignnone size-full wp-image-2262" src="/assets/images/uploads//2017/01/boxifier-update.jpg" alt="" width="800" height="287" srcset="/assets/images/uploads//2017/01/boxifier-update.jpg 800w, /assets/images/uploads//2017/01/boxifier-update-300x108.jpg 300w, /assets/images/uploads//2017/01/boxifier-update-768x276.jpg 768w" sizes="(max-width: 800px) 100vw, 800px" />

The only caveat is that you need to download the latest version manually to run it. This <kbd>autohot key</kbd> checks the latest version in your computer and then compares it with the latest version available on the official website of boxifier. If new version is found, then it downloads the Latest setup and installs it automatically.
  
You can autorun it on startup or can manually run it.

## Steps

  1. You need to install AutoHotKey from  `<a href="https://autohotkey.com/download/ahk-install.exe">Download Link</a>` 
  2. Install it.
  3. If you don&#8217;t want to install it, then You can download the directly compiled version <a href="https://github.com/1nsp1r3rnzt/Boxifier-AutoUpdate-AutoHotKey/releases/latest" target="_blank">Here</a>
  4. Else, to run from the source, you need to click on the Ahk file to run it. Download the script <a href="https://github.com/1nsp1r3rnzt/Boxifier-AutoUpdate-AutoHotKey" target="_blank">Download Boxifier AutoUpdate.ahk</a>

## Source Code

<pre class="theme:xcode lang:default decode:true">;verison 0.2


#NoEnv  ; Recommended for performance and compatibility with future AutoHotkey releases.
; #Warn  ; Enable warnings to assist with detecting common errors.
SendMode Input  ; Recommended for new scripts due to its superior speed and reliability.
SetWorkingDir %A_ScriptDir%  ; Ensures a consistent starting directory.
SetControlDelay -1
;things to do,  check periodically, gui
;check and deleted if last version file cache is present

boxicheckfile=boxifierv
UrlDownloadToFile, http://www.boxifier.com/, %boxicheckfile%.txt
;read downloaded source into variable
FileRead, checkversionsource, %boxicheckfile%.txt
;find position
Foundpos := RegExMatch(checkversionsource,"Download Boxifier (\d\.\d\.\d{1,2}) for Windows", Version)
;check the local version present; i assume it is installed in default location
BoxifierLoc = %A_AppData%\Boxifier\Boxifier.exe
FileGetVersion, BoxifierLocalVer, %BoxifierLoc%

; Count the decimals in the online version
count = 0

Loop, Parse, Version1, .
{
 count += 1
}

actualcount := count - 1

countloc = 0
; Count the decimals in the local version

Loop, Parse, BoxifierLocalVer, .
{
 countloc += 1
}

actualcountloc := countloc - 1
;if both version are not equal in case as local version has one more decimal as 1.5.24.0 while online has 1.5.24
if(actualcount!=actualcountloc)
{
LastDotPos := InStr(BoxifierLocalVer,".",0,0)  ; get position of last occurrence of "."
BoxifierLocalVer2 := SubStr(BoxifierLocalVer,1,LastDotPos-1)  ; get substring from start to last dot
}
else
{
BoxifierLocalVer2:=BoxifierLocalVer
}

if (version1== BoxifierLocalVer2)
 {
 msgbox, You have the latest version Boxifier - %version1% installed.

 
 }
 else
 
 {
;url to download the file
urltodownload = http://www.boxifier.com/Boxifier-Setup-%version1%.exe
UrlDownloadToFile, %urltodownload%, Boxifier-%version1%.exe
;run the downloaded file
run, Boxifier-%version1%.exe
sleep 2000
;further install it 
IfWinExist, Setup - Boxifier
WinActivate ; use the window just found above
sleep 2000
send {Tab}
Send {Up 1}
send {enter}
msgbox, installed
}
;Deleted downloaded html page
 IfExist, %A_ScriptDir%\%boxicheckfile%.txt
{
FileDelete,%A_ScriptDir%/%boxicheckfile%.txt
}</pre>

&nbsp;

This solves the problem of updating boxifier manually.