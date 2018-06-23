---

title: Anki Quick Adder &#58; A chrome extension to add words to Anki desktop quickly
date: 2018-05-26T21:57:27+00:00
permalink: /chrome-anki-quick-adder/  
comments: true
layout: splash
image:
  path: /assets/images/uploads/2018/06/anki-add-cards-quickly.png
categories:
  - programming
tags:
  - javascript
  - chrome 
classes: wide
sidebar:
  title: "Sample Title"
  nav: sidebar-sample


header:
  teaser: /assets/images/uploads/2018/06/anki-add-cards-quickly.png

  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/uploads/2018/06/AnkiQuickAdder.png
  cta_label: "<i class='fas fa-download'></i> Install Now"
  caption:
  cta_url: "https://chrome.google.com/webstore/detail/anki-quick-adder/gpbcbbajoagdgnokieocaplbhkiidmmb"
excerpt: 'A Google Chrome extension for Anki.  Perfect for creating the flash cards directly from Google Chrome on your Anki Desktop. <br /><small><a href="#demo">View Demo</a></small>  <br /><br /> {::nomarkdown}<iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=1nsp1r3rnzt&repo=chrome-anki-quick-adder&type=star&count=true&size=large" frameborder="0" scrolling="0" width="160px" height="30px"></iframe> <iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=1nsp1r3rnzt&repo=chrome-anki-quick-adder&type=fork&count=true&size=large" frameborder="0" scrolling="0" width="158px" height="30px"></iframe>{:/nomarkdown}'
intro: 
  - excerpt: 'Get notified when I update the extension. &nbsp; [<i class="fab fa-twitter"></i> @king99immortal](https://twitter.com/king99immortal){: .btn .btn--twitter}<br> **Features**'
feature_row:
  - image_path: /assets/images/uploads/2018/06/chrome-menu.png
    alt: "Add card to Chrome"
    title: "Chrome Menu"
    url: "chrome-anki-quick-adder/#from-chrome-menu"
    btn_label: "Read More"
    btn_class: "btn--primary"
    excerpt: "Quick chrome menu allows you to add a card with by selecting a word and right clicking on the field name."
  - image_path: /assets/images/uploads/2018/06/shortcuts.png
    alt: "Customizable Shortcuts"
    title: "Customizable Shortcuts"
    excerpt: "You can set shortcuts for your favourite deck and models. Customizable shortcuts allows adding data quickly."
    url: "chrome-anki-quick-adder/#shortcuts"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/uploads/2018/06/tags-2.png
    title: "Auto-complete Tags"
    url: "chrome-anki-quick-adder/#inline-editor"
    btn_label: "Read More"
    btn_class: "btn--primary"
    excerpt: "Auto-complete tags makes it a breeze to tag notes quickly. Plus, In-line editor helps to customize notes."

---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

## Demo
{% include video id="3oV5pkt20DU" provider="youtube" %}

<a href="https://github.com/1nsp1r3rnzt/chrome-anki-quick-adder/fork" class="github-corner" aria-label="View source on Github"><svg width="80" height="80" viewBox="0 0 250 250" style="fill:#151513; color:#fff; position: absolute; top: 75; border: 0; right: 0;" aria-hidden="true"><path d="M0,0 L115,115 L130,115 L142,142 L250,250 L250,0 Z"></path><path d="M128.3,109.0 C113.8,99.7 119.0,89.6 119.0,89.6 C122.0,82.7 120.5,78.6 120.5,78.6 C119.2,72.0 123.4,76.3 123.4,76.3 C127.3,80.9 125.5,87.3 125.5,87.3 C122.9,97.6 130.6,101.9 134.4,103.2" fill="currentColor" style="transform-origin: 130px 106px;" class="octo-arm"></path><path d="M115.0,115.0 C114.9,115.1 118.7,116.5 119.8,115.4 L133.7,101.6 C136.9,99.2 139.9,98.4 142.2,98.6 C133.8,88.0 127.5,74.4 143.8,58.0 C148.5,53.4 154.0,51.2 159.7,51.0 C160.3,49.4 163.2,43.6 171.4,40.1 C171.4,40.1 176.1,42.5 178.8,56.2 C183.1,58.6 187.2,61.8 190.9,65.4 C194.5,69.0 197.7,73.2 200.1,77.6 C213.8,80.2 216.3,84.9 216.3,84.9 C212.7,93.1 206.9,96.0 205.4,96.6 C205.1,102.4 203.0,107.8 198.3,112.5 C181.9,128.9 168.3,122.5 157.7,114.1 C157.9,116.9 156.7,120.9 152.7,124.9 L141.0,136.5 C139.8,137.7 141.6,141.9 141.8,141.8 Z" fill="currentColor" class="octo-body"></path></svg></a><style>.github-corner:hover .octo-arm{animation:octocat-wave 560ms ease-in-out}@keyframes octocat-wave{0%,100%{transform:rotate(0)}20%,60%{transform:rotate(-25deg)}40%,80%{transform:rotate(10deg)}}@media (max-width:500px){.github-corner:hover .octo-arm{animation:none}.github-corner .octo-arm{animation:octocat-wave 560ms ease-in-out}}</style>

## Installation

1. Download [Anki](https://apps.ankiweb.net) for your platform.

Please *start Anki* before running chrome or before installing chrome extension.
{: .notice--danger}


2. Install [ankiConnect](https://ankiweb.net/shared/info/2055492159)
- Please [see note for windows](https://github.com/FooSoft/anki-connect#notes-for-windows-users) users to allow ankiConnect.
- Mac users need to **[follow these instructions](https://github.com/FooSoft/anki-connect#notes-for-mac-os-x-users)** to allow communication.
3. Restart Anki 
4. install [extension from webstore](https://chrome.google.com/webstore/detail/anki-quick-adder/gpbcbbajoagdgnokieocaplbhkiidmmb)
5. See known [bugs and issues](#known-bugs-and-solutions) in this readme to solve any bugs.

## Getting Started
Scroll ⬆️ for setup process, if you haven't set it up yet.
You can add cards through extension pop-up or chrome menu.
- For the first time, click extension ![icon][icon] icon.
- Please, select a deck and note type before adding cards for the first time.



# Add from Popup

![image-left](/assets/images/uploads/2018/06/ankiStep1.png){: .align-left}
## Steps
You can add cards by `clicking` the ![icon][icon] in chrome.
1. Run Anki. 

On successful connection, it will show decks and models.
{: .notice--info}

2. Click App icon to open app.  
3. Select Deck type.
4. Select Card type.
5. Enter the data in fields.
6. (Optional) Enter tags separated by ; for auto-complete.
7. Click Add Note.

<div class="cf"><hr></div>

<!-- links -->
   [icon]: /assets/images/uploads/2018/06/icon-32.png 
<!-- linksend -->
# From Chrome Menu

![image-right](/assets/images/uploads/2018/06/anki-2.png){: .align-right}

### steps
If you cannot find this menu, then [click here to read more.](#known-bugs-and-solutions)

1. Select the `word`, you want to enter.
2. Right click and select `Add to Anki`
3. Click the `field name` like `add to text` to send the word to that field.
4. Select, another word and add it to other field.
5. Right click and Click submit. [You can also use shortcuts](#shortcuts)
7. A popup will open to submit your data for 2 seconds and will close.

<div class="cf">
While in Sync, Mode. Chrome Menu is available only, when Anki is running in background.
<hr></div>

# Add From shortcuts

1. 🛑 You need to setup shortcuts.

[Read here](#modify-above-shortcuts) about setting shortcuts.

2. Select the desired text to add.
3. press the shortcut to add it to the field.



## Inline editor

![image-left](/assets/images/uploads/2018/06/anki-inline-editor.png){: .align-left }

### Steps to use Inline editor

Inline editor, is used to change color of text on the go.

1. Click app icon ![icon][icon]
2. Write text in any field like `Front` or `Back`
3. select the word to change options like `color`,`bold`,`italics`,`underline`. 
4.  A toolbar will open to edit the word.

The shortcut for creating `cloze` is not in tool bar.
To create a cloze, select the word or sentence and press `Alt Shift w` .
{: .notice--danger }
<div class="cf"><hr></div>


## Append Mode

[![image-left](/assets/images/uploads/2018/06/anki-quick-adder-append-mode.png)](/assets/images/uploads/2018/06/anki-quick-adder-append-mode.png){: .align-left}
### Steps to use Inline editor

Append mode is useful for adding text to same field, from `chrome menu` 
1. Switch on the append settings.
2. Select the word, you want to enter.
3. Click the field to send the word to that field.
4. Select another data.
5.  Right click and click on the same add to field
5.  Click the submit button through popup or chrome menu.

<div class="cf"><hr></div>

## Install AnkiConnect

1. Open the Install Add-on dialog by `selecting Tools > Add-ons > Browse & Install` in Anki.
2. Input `2055492159` into the text box labeled Code and press the OK button to proceed.
3. Restart Anki when prompted to do so in order to complete the installation of AnkiConnect.

Anki must be kept running in the background in order for other applications to be able to use AnkiConnect. You can verify that AnkiConnect is running at any time by accessing `localhost:8765` in your browser. If the server is running, you should see the message AnkiConnect v.6 displayed in your browser window.
{: .notice--danger}

## Settings

**Sync Settings** 🆕 

Manual: caches lists & provides a button  to refresh manually. (faster)    
Live: updates Deck, model list when extension pop-up is opened every time. (slow)

**Favourite Deck:** 🆕  
- Select Your favourite deck
- Press `ALT+SHIFT+d` to select favourite deck.

**Favourite Model:** 🆕  
- Select Your favourite model
- Press `ALT+SHIFT+c` to select favourite model.

**paste Plain text:** 🆕  
paste plain text.

**Clean pasted Html** 🆕  
cleans html, for example elements with  `class and dir` from text.

**Append:**
 Append fields data from chrome menu instead of overwrite.

**Rebuild Chrome Menu**  
Recovers chrome menu, if it crashed.


**Debug:**  
 Turn console debug on or off

**Sync**  
 Anki Desktop to AnkiWeb(Opens Anki Desktop)  

**Clear all Settings & Restore defaults**  
Delete all settings and restore defaults.

# Shortcuts
There are two types of shortcuts.

## Shortcuts for pop-up 🆕

After setting up.
1. click ![icon][icon] for opening extension.
2. click settings. 
2. Select your favourite `deck` and `model`.

now, While adding a new card, in pop-up

| Purpose         | Shortcut      |Modifiable|
| ------------- |:-------------:| -----:|
|Select the **favourite deck**|`alt shift d`  | Yes| 
|Select the **favourite model**|`alt shift c`   |Yes| 
|Create a  ** cloze in a field for selected text**|   `alt shift w` |Yes| 
|Quick Submit (will add the card to anki): |`ctrl enter` |Yes| 
|New Line : |`shift enter` |No|
|New paragraph (use New line shortcut if you don't want paragraph): |`Enter` |No|

## On any page you browse. 🆕

| Purpose         | Shortcut      |Modifiable|
| ------------- |:-------------:| -----:|
|Send selected text to **field 1**|`alt shift 1`  | Yes| 
|Send selected text to **field 2**|`alt shift 2`   |Yes| 
|Send selected text to **field 3**|   `alt shift 3` |Yes| 
|Quick Submit (will add the card to anki): |`alt shift 4` |Yes| 

These shortcut will only be assigned if you have not assigned these buttons to any other extension before.
To be sure, follow below instructions.
{: .notice--danger }

## Modify above shortcuts
1. Goto extensions in Google Chrome.
2. Click on `keyboard shortcuts`.

⚠️ If you can't find it, copy `chrome://extensions/shortcuts` and paste in address bar. 
{: .notice--info}

It will open setting similar to below image.
![image](/assets/images/uploads/2018/06/shortcut-extension.png)

You can change shortcuts according to your needs.

## Known Bugs and Solutions 

| Bug           | Solution      | Reason  |
| ------------- |:-------------:| -----:|
| chrome Menu disappears      | ![enter image description here](https://raw.githubusercontent.com/1nsp1r3rnzt/chrome-anki-quick-adder/master/docs/images/no-menu.png)<br> 1. Start Anki <br> 2. Goto extension settings. <br> 3. Settings> Click Rebuild Menu  | 1. Anki is not running.<br>2. Chrome was opened before running Anki |
|  Duplicate Note. Note not Added.     | Change main field as Anki doesn't allow duplicate notes.   |   Note is already present in Anki |
|  No notification on Mac on successful card addition.   |   no solution yet |need mac  to test so not fixable yet.|

## Latest Update

<div style="color: orange;">The extension has been updated to latest version 1.0.4</div>  
This version provides
- Ability to export and import your saved notes in extension.
- fixed typeError bug on saving notes.
- Quick icon to turn off global sticky fields.

previous versions

- Fixed bug for users who updated extension.

- Ability to save notes in Local Storage and sync later. (settings-> **saveNotes**) [demo](https://imgur.com/a/G2dYuOP)
- Added ability to customize in-line editor buttons (settings-> **In-Line editor Buttons**)
- Added sticky Fields. Click [S] and field data will persist after adding a note until you clear.[demo](https://imgur.com/a/KpAFxe7)
- Mode to change field background theme to dark mode temporarily.
- Fixed field deletion on noteType change.

- Toggle between favorite decks or models (select more than one deck or model) [Open demo](https://imgur.com/a/o54jyFw)
- Fixed cloze caret position while adding from shortcut.
- Customizable shortcuts for decks, models, cloze and quickSubmit.

### Full changeLog                    
                                      Version 1.0.4 - Tuesday, June 19th, 2018
                                        - Ability to export and import your saved notes in extension.
                                        - fixed typeError bug on saving notes.
                                        - Quick icon to turn off global sticky fields.
                                        --------------------------------
                                        Version 1.0.3 - Tuesday, June 19th, 2018
                                        - Moved to local storage to save currentFields instead of sync
                                        --------------------------------
                                        Version 1.0.2 - Tuesday, June 19th, 2018
                                        Fixed Type Error 
                                        ---------------------              
                                        Version 1.0.1 - Tuesday, June 19th, 2018
                                          - Fixed settings bug for users who updated extension.
 
                                          -----------------------------------
                                   Version 1.0.0 - Monday, June 18th, 2018
                                          - Ability to save notes in Local Storage and sync later. (settings-> saveNotes)
                                          - Added ability to customize in-line editor buttons (settings-> In-Line editor Buttons)
                                        - Added sticky Fields. Click [S] icon and field data will persist after adding a note until you clear.
                                        - Mode to change field background theme to dark mode temporarily.
                                        - Fixed field deletion on noteType   change.
                                        ---------------------------------------
                                          Version 0.0.8 - Sunday, June 10th, 2018
                                          - Toggle between favourite decks or models (select more than one deck or model)
                                          - Fixed cloze caret position
                                          - Customizable shortcuts
                                        ---------------------------------------Version 0.0.7 - Wednesday, June 7th, 2018
                                          - card submission directly on shortcut instead of submission through pop-up.
                                        ---------------------------------------Version 0.0.6 - Wednesday, June 7th, 2018
                                        -fixed settings bug for users who updated instead of installing it.
                                        ---------------------------------------Version 0.0.5 - Wednesday, June 6th, 2018
                                        ---------------------------------------
                                        - shortcuts for: deck, model and Cloze
                                        - shortcuts for: adding selection to fields
                                        - Cache for: decks, models and tags
                                        - settings for: cleaning text
                                        - Settings for: submit timeout from chrome menu
                                        - 

                                          Version 0.0.4 - Sunday, June 3rd, 2018
                                        ---------------------------------------
                                        - Fixed adding cards from context menu

                                            --------------------------------------------------
                                        Version 0.0.3 - Sunday, June 3rd, 2018
                                        -----------------------------------------------------------------------------------------
                                        - Fixed appendMode
                                        - Added setting to turn on debugging.
                                                 
                                        Version 0.0.2 - Saturday, June 2nd, 2018
                                        -----------------------------------------------------------------------------------------
                                        - Fixed note adding error on windows and mac
                                        
                                        -----------------------------------------------------------------------------------------
                                        Version 0.0.1 - Friday, June 1, 2018
                                        -----------------------------------------------------------------------------------------
                                        - Released beta version
                                        -fixed deck selection for single decklist
                                        -fixed deck selection for modelList
                                        - parsed tags for autocomplete




## Contributing

>

### Step 1

- **Option 1**
    - 🍴 Fork this repo!

- **Option 2**
    - 👯 Clone this repo to your local machine using `https://github.com/1nsp1r3rnzt/chrome-anki-quick-adder.git`

### Step 2

- **HACK AWAY!** 🔨🔨🔨

### Step 3

- 🔃 Create a new pull request using <a href="https://github.com/1nsp1r3rnzt/chrome-anki-quick-adder/compare/" target="_blank">`new pull request`</a>.

---

## License

- **[MIT license](/LICENSE)**
- Copyright 2018 © <a href="http://codehealthy.com" target="_blank">Ranjit Singh</a>.
