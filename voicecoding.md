---
layout: page
title: Voice coding
---
# Caster
[Caster](http://dictation-toolbox.github.io/caster/) is a collection of tools aimed at enabling programming and accessibility entirely by voice built upon Natlink and the [Dragonfly](https://github.com/dictation-toolbox/dragonfly) API. It is available on Windows and requires Dragon.

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
[Talon](talonvoice.com) aims to bring programming, realtime video gaming, command line, and full desktop computer proficiency to people who have limited or no use of their hands, and vastly improve productivity and wow-factor of anyone who can use a computer.

It is currently available on OS X and requires Dragon Dictate.

{% include youtubePlayer.html id="HsodtJY0BX8" %}