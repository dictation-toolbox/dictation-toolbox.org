---
layout: page
title: Voice coding
---
# Caster
[Caster](https://caster.readthedocs.io/en/latest/) is a collection of tools aimed at enabling programming and accessibility entirely by voice built upon Natlink and the [Dragonfly](https://github.com/dictation-toolbox/dragonfly) API. It is available on Windows and requires Dragon.

Caster provides three key types of command:
* Universal navigation and editing - These commands are active all the time, and provide input commands for letters, numbers and punctuation, as well as the ability to easily manipulate windows and text. 
    - `window right` moves the active window to the right-hand side of the screen.
    - `prekris` inserts a pair of brackets `()` and moves the cursor inside them.
    - `shackle` selects the current line.
* Application specific control - These commands are only activated when a particular program is the active window, and they provide support for text editors, IDEs, web browsers etc. For example, while the Sublime text editor is the active window, saying
    - `find` will execute a `ctrl-f` keystroke, bringing up the find and replace prompt,
    - `open file` will execute a `ctrl-o` keystroke,
    - `edit next <n>` - `ctrl-d` n times, selecting the next n instances of the currently selected word.
* Language specific coding - These modules are activated and deactivated with the `enable/disable <language>` voice command and contain language specific commands for inputting code. For example, saying `enable python` will enable the following commands. 
    - `for loop` which will insert `for i in range(0, ):`
    - `print to console` - `print()`
    -  `open file` -  `open('filename', 'r') as f:`

# Talon
[Talon](https://talonvoice.com/) aims to bring programming, realtime video gaming, command line, and full desktop computer proficiency to people who have limited or no use of their hands, and vastly improve productivity and wow-factor of anyone who can use a computer.

It is currently available on OS X and requires Dragon Dictate.

{% include youtubePlayer.html id="HsodtJY0BX8" %}


# Vocola
[Vocola](http://vocola.net/) is a voice command language - a language for creating commands to control a computer by voice. Two versions are available: Vocola 2 works with Dragon NaturallySpeaking (DNS) and Vocola 3 works with Windows Speech Recognition (WSR) on Windows 8, 7, and Vista. While DNS and WSR handle the heavy lifting, Vocola (pronounced "vo-CO-luh") concentrates on features and ease of use. In particular, Vocola offers the following:

Easy to use:

* Simple, concise command syntax - most commands are one-liners
* Easy to view and modify commands
* Changed commands are loaded automatically
* Large set of useful sample commands
* Free

Features:

* Create commands which capture any dictated words
* Use concise number ranges, optional words, and inline word lists
* Specify different actions for variable words
* Speak a continuous sequence of commands
* Re-use work with include files and user-defined functions


[https://docs.google.com/document/d/e/2PACX-1vSGRicRTJ2iv7rzLnwYxGnUb39usUk_5o2KPxJ5YE91qv-W_lWHD1C7S4syAHM61VAheR5lQ6hoE55W/pub](Getting started with voice coding in Vocola)