# Songlist Reveal

Songlist Reveal is a simple slideshow controller designed to display song lyrics for projector or multple display. It reads and parse songlist.txt which contains slideshow data with songlist syntax then translate it into compatible reveal.js HTML elements. 

This controller can launch another instance of songlist window that act as presentation view that follow slide changes of controller window. Some functionality like background change is simply implemented by drag and drop the image file to controller window to change both controller and presentation window.


## Installation

You need to have Bower installed. 
`brew install bower`

Once you clone this repo, you can run

`bower install`


## Firefox Config

1. Type "about:config" on the address bar.
   (Click "I Accept The Risk" button when the warning come out)

2. Enter "security.fileuri.strict_origin_policy" on the Search box

3. Double click the item value from true to  false


## songlist.txt Syntax


### New page
Put `>` to start a new page (let's call this page break delimiter).

Example:

    >Verse 1
    This is the verse 1 on page 1

    >Verse 2
    This is the verse 2 on page 2

### New Section
Put `>-` To start new section or new song title.

    >-Song Title
    (the cool song)

    >Lyric line 1
    Lyric line 2


### Inserting HTML

You can add HTML on each page by simply put the html tags after the page break delimiter

### Background Video

To put background video you need to put the mp4 video inside `videos` folder. Open videos folder with windows explorer or finder and then drag and drop the video file to the main presentation control window. 
