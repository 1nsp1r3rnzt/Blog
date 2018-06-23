---
id: 2358
title: 'Automating The Course Registration Process  at My University: A story about problem solving'
date: 2017-09-05T01:16:52+00:00
permalink: /automating-the-course-registration-process-at-my-university-a-story-about-problem-solving/
header:
  teaser: /assets/images/uploads/2017/09/course-registration-fail-meme.jpg
categories:
  - AutoHotKey
---
Carleton University has a different registration process than University of Ottawa. It has a concept of [time ticket](https://carleton.ca/registrar/registration/timeticket-information/time-tickets/) **(which sucks)** where your course registration opens at a specific time, while all students of Uottawa can register courses at the same time. Also, the registration of Fall and Winter courses are done together so you are out of luck if your time ticket is not the earliest. ![image](/assets/images/uploads/2017/09/course-registration-fail-meme.jpg) 

I faced same situation when my time ticket was during afternoon. Moreover, to rub salt in the wound, one of the course was removed from my registration as it was not longer offered. I found this 3 days later and was left with only two courses in my portal. The only option was to check the course status continuously and hope for someone to drop the course.

> I don't think necessity is the mother of invention. Invention . . . arises directly from idleness, possibly also from laziness. To save oneself trouble. ~ Agatha Christie

 This laziness lead me to automate the process of course registration which monitors desired course’s status. It registers the course as soon as someone drops the course or when it becomes available. The Main GUI is as below. The software is written using [Autohotkey](https://autohotkey.com/docs/AutoHotkey.htm) scripting language. ![](/assets/images/uploads//2017/09/main-pagee.png) 

 When a course is registered successfully, the user is notified instantly using [Pushbullet’s API](https://docs.pushbullet.com/) which send and receive messages from computer to your mobile phone and vice versa.

 Most of the settings are stored and retrieved on next run of the software. ![](/assets/images/uploads//2017/09/settings.png)

  Brief logic of the software is as below.   ![](/assets/images/uploads//2017/09/Drawing1-1.png)    

   The happiest moment was when it registered the desired course for me and sent me a notification on my phone which was set to play 🚀 rocket sound 🚀 upon receiving successful registration. Please send me an email or comment if you want to try the software for demonstration purpose.

Credits: 
The encryption library used for storing Student’s username and Password is provided by user [Dra’Gon](https://autohotkey.com/board/topic/23097-encryptiondecryption/) on Authotkey forums.