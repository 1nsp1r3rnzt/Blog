---
title: 'Quick Guide: Edit Evernote Notes In SublimeText Using MarkDown'
date: 2017-02-05T14:17:15+00:00
permalink: /evernote-notes-in-sublime-text/
header:
  teaser: /assets/images/uploads//2017/01/pexels-photo-240038-copy.jpg 
categories:
  - AutoHotKey
---
Markdown is a simple markup language which supports adding formatting to plain text. It has minimalistic approach as compared to HTML
 ![](/assets/images/uploads//2017/01/pexels-photo-240038-copy.jpg) 

 Sadly, Evernote does not support Markdown editing in its native application. The options are to download Marxico app or other chrome extensions. The best option for those who use sublime text is to install `[Sublime-Evernote](https://github.com/bordaigorl/sublime-evernote)` extension. 

 The key binds are disabled by default. You need to edit `Preferences >Key Binding` and Paste the Following
 {%gist 44568b64c7cac5a729ea12b8eb78f7fe %}

 To OverWrite a note, You need to press `CTRL + E S`

To Send a new note, You need to press `CTRL + E U `

 Download the following AutoHotkey Script to quickly open notes in sublime text. You need to download Autohotkey to run the script.
 {%gist f47044c6f65880d9f113ab75132a18ef %}

  The default key for opening note with Sublime text is `CTRL + M.` Press the key when you are on the snippet view in Evernote. Here is the preview. You can click image to enlarge.

![Preview of editing notes](/assets/images/uploads//2017/01/Markdown-evernote-sublime-shortcut-demo.gif)

It will open note quickly if sublime Text is already opened.