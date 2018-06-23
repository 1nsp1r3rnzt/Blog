---
title: Enhancing podcast note taking Process on Android 
date: 2018-05-15T17:01:27+00:00
permalink: /podcast-note-taking-app-android/
categories:
  - Android
tags:
  - Tasker
  - Automation
---
Listening podcasts is advantageous as it provides deep insight into the lucid life experience of others.

I struggled to take notes while listening to the podcasts as a normal podcast is usually 1-3 hours long and I always listened to it over several days.

This prompted me to find a solution to store notes in an organized way and the most efficient method is to utilize Evernote for storing podcast notes.

## Demo:

{% include video id="WBRIIv738lQ" provider="youtube" %}


<div class="notice--warning">
  The secret here is to append the notes for the same podcast which allows the flexibility to listen to the podcast in several days.
</div>

I have created a Tasker app which allows you to add notes.

{% capture notice-2 %}
[Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en) 

[Podcast Addict](https://play.google.com/store/apps/details?id=com.bambuna.podcastaddict&hl=en_CA) 


[Evernote](http://evernote.com) 

[MailTask plugin](https://play.google.com/store/apps/details?id=com.balda.mailtask&hl=en) for tasker or any mail plugin 

[AutoNotification](https://play.google.com/store/apps/details?id=com.joaomgcd.autonotification&hl=en_CA) 

[Material Design plugin](https://play.google.com/store/apps/details?id=com.nick.mowen.materialdesignplugin&hl=en)
{% endcapture %}

<div class="notice--warning">{{ notice-2 | markdownify }}</div>


## Setup: 
1. Download Project: [Github Link](https://github.com/1nsp1r3rnzt/Tasker-Apps/tree/master/Notes%20Adder%20Podcast%20Addict) 
2. Import project in tasker 
3. open the evernotemainApp task and set up your task as described in the image below.
  
    ![setup Tasker](/assets/images/uploads//2018/05/Setup-tasker-podcast-addict.jpg)

  4. If you use Nova Launcher, then just add the task evernoteMainApp as a swipe gesture on podcast addict app or have the shortcut of the task on homescreen,

  5. Open podcast Addict and then run the task. Here is the screenshot of the task.

  6. ![screenshot2](/assets/images/uploads//2018/05/workflow-evernote-podcast-addict.jpg)
  7. Click ok and it will send an email to evernote which add the note to your evernote notebook with the specified tags.

## **Final Result**

![Final result](/assets/images/uploads//2018/05/podcast-imrpovement-notes.png)
The notes are stored in evernote.
