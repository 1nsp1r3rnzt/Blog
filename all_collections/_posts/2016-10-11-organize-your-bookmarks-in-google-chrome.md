---
id: 2122
title: 'Best &#038; Minimal Way To Organize Your Bookmarks In Google Chrome: Humble New Page'
date: 2016-10-11T04:02:38+00:00
show_author: true
header:
  teaser: "/assets/images/uploads/2016/10/bookmarks.png"
image:
  path: "/assets/images/uploads/2016/10/bookmarks.png"
permalink: /organize-your-bookmarks-in-google-chrome/
categories:
  - google-chrome
tags:
  - chrome-extension
---
Organizing your bookmarks can be a challenging task, especially when you are a information junkie like me.

I have tried options like making custom html page but static page makes it difficult to edit quickly. Other options include different extension and the best and minimal one is [Humble New Page.](https://chrome.google.com/webstore/detail/humble-new-tab-page/mfgdmpfihlmdekaclngibpjhdebndhdj?hl=en)
  
Here is the preview of what you will achieve after installing it and then using some CSS modifications. (You can click to enlarge the preview)
  
![preview of modifications](/assets/images/uploads//2016/10/Untitled.gif)

It is a drag and drop extension. You need to divide your bookmarks into different categories. The  <kbd>folder name</kbd> is used as a heading when you drag two folders in a column else it will display the links of the folder if a single folder is dragged.

![Final Result](/assets/images/uploads//2016/10/bookmarks.png)

For column displaying single folder like the fourth column, you need to make a new bookmark with the URL containing the value as ` http://127.0.0.1/myownbookmarks`

Then go to settings in extension and then advanced>custom CSS and paste the following code.

{% gist 4d80123d82fb3339326682174ed6e47f HumbleNewPage.css %}

