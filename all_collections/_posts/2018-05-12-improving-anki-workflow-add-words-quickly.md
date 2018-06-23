---
title: Improving Anki Workflow on Windows to Add words Quickly
date: 2018-05-12T17:53:41+00:00

permalink: /software-for-improving-anki-workflow-on-windows-to-add-words-quickly/
excerpt: Anki is a flashcard-based software. It accelerates the p[...]
header:
  overlay_color: "#333"
  og-image: /assets/images/uploads/2018/05/anki-workflow-1.jpg
classes: wide
categories:
  - Software
tags:
  - Automation
---
Anki is a flashcard-based software. It accelerates the process of learning by helping to retain information in the long-term memory.

The concept of utilizing Anki for improving vocabulary is hindered by the burden which comes with the cumbersome process of adding words to it.
  
The usual workflow needs you to add the word, meaning, and a sentence.
![workflow](/assets/images/uploads//2018/05/anki-workflow-1.jpg)

The flow is interrupted as you have to stop reading an article and add the word to Anki.

This software automates the process of adding the word and the sentence where you read the word quickly to Anki.

## Quick Demo and Video Tutorial

{% include video id="H3pl5dh0YHg" provider="youtube" %}

### Demo Screenshot
  
[![screenshot](https://raw.githubusercontent.com/1nsp1r3rnzt/Anki-Quick-Word-Adder/master/images/picture.png)

Additional features include retrieving images automatically related to the word from two sources if available.

## Getting started

Download the source code at  [GitHub project repo.](https://github.com/1nsp1r3rnzt/Anki-Quick-Word-Adder)


**Please backup and sync Anki before proceeding.**

**Steps**

1. Click the StartApp file to start the setup.
2. It installs the demo deck which has the 3 fields card type. Anki needed to be installed at demo location for the software to work.
3. Then, you need to setup Oxford Dictionary API
````
global APP_ID:=""
global APP_KEY:=""
````
4. Finally, run, StartApp.ahk to start the software
5. press **\`** to run the software. The shortcut can be changed in StartApp.ahk

## Prerequisites

<div class = "notice--danger" markdown="1">

Anki: [Anki Download](https://apps.ankiweb.net/) 

AutohotKey: [AutohotKey Download](https://autohotkey.com)

Oxford Dictionary API [Oxford Dictionary API](https://developer.oxforddictionaries.com/)

[Google Chrome Dictionary Extension](https://chrome.google.com/webstore/detail/google-dictionary-by-goog/mgijmajocgfcbeboacabfgobmjgjcoja?hl=en) – optional

</div>

### **<span style="text-decoration: underline;">Other points to consider for learning effectively</span>**

  Benny Lewis, the Irish polyglot emphasizes the importance of associating images and learning words by speaking with native speakers along with SRS. This inspired me to find a way to add images automatically with each word.

Further, [Olle Linge](https://www.hackingchinese.com/if-you-think-spaced-repetition-software-is-a-panacea-you-are-wrong/) discusses the downside about relying only on spaced repetition method to learn and retain information such as.

  * It’s spaced repetition, not spaced learning.
  *  it’s efficient doesn’t mean you should learn everything with it
  * SRS is a tool, not a comprehensive learning method

  * SRS is a flexible tool, use it wisely

  For programming, The concept of spaced repetition method is quite useful described by <a href="https://sivers.org/srs">Derek Sivers. </a>

> I’ve been doing this for a year, and it’s **the most helpful learning technique I’ve found in 14 years of computer programming**.~Derek Sivers

Derek points out to

  1. First, learn!  ~ Always add the card after learning the concept.
  2. Convert Knowledge into Small Facts: ~ Breaking the question down to [5ws](https://en.wikipedia.org/wiki/Five_Ws)
  3. Try to trick your future self ~ Adding a question in a creative and more than one way
  4. Run Through it Daily: making it a habit


<div class="notice--success">
This will help to turn Anki into a useful resource for learning rather than using it for rote learning.  
</div>
