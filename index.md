---
layout: page
title: Home
---

Here we want you to get you started with voice programming! We will introduce you to the most commonly used toolchain for voice programming but at the same time give you some pointers  to alternative projects.

# Project Overview
Voice programming has been  growing around the commercial voice recognition software [Dragon](https://www.nuance.com/dragon.html).  Dragon takes your voice and tries to translate that into written text. In order to control our system by voice we need to be able to create our own commands to do things like map the speech snippet "save file" to "ctrl+s". Fortunately Dragon implements a COM (C/C++)  API that allows us to create our own commands. Since c++ is not a very convenient scripting language Natlink   translates the   API to Python. However this  API is still fairly  hard to use and  even worse it is specific to the voice-recognition-engine Dragon. Yet another project, Dragonfly,  tackles this tasks and  not only makes  it much easier to create your own commands but also allows you to  use a different voice recognition engine like [Kaldi](https://kaldi-asr.org/doc/about.html) or Windows speech recognition (WSR). Finally there is a host of projects that depend on Dragonfly that aim to provide the user with sensible defaults commands  to control the system and even commonly used programs like Firefox, Thunderbird or Intelji-IDEs.

 <img src="{{ site.baseurl }}/assets/img/voicecoding_landscape.svg"  >
 
 