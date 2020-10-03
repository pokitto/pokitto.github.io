---
title: Quick software setup
has_children: false
permalink: /start/learn/quickstart/step1
parent: Quick Start Guide
nav_order: 1
---

# Step 1: Download and install FemtoIDE
FemtoIDE is an Integrated Development Environment (IDE), which combines all the tools you need to create softwares for Pokitto in a single graphical user interface (GUI). FemtoIDE consists of:
- Source code editor: with features such as syntax highlighting, and auto-completion.
- Build automation.
- Debugger: supports both PokittoEmu and Segger J-Link hardware debuggers.
- Pokitto emulator.
- Sprite Editor.

[more info about FemtoIDE...](https://talk.pokitto.com/t/tool-femtoide/1832)

---
# Download
Simply download the right one according to your operating system and proceed to installation.  
[Download it from here](https://github.com/felipemanga/FemtoIDE/releases/latest)

---
# Installation

## Windows
Extract the zip and run `IDE.exe`.

## Macintosh


## Fedora
Before you can run the IDE's emulator, you must download the SDL2 libraries with the following command: 
```
sudo dnf install SDL2 SDL2_net SDL2_image
```

Once that's done, extract the Linux release and run IDE.

## Debian / Ubuntu
Before you can run the emulator, you must download the SDL2 libraries with the following command:
```
sudo apt install libsdl2 libsdl2_net libsdl2_image
```

Once that's done, extract the Linux release and run IDE.

In case you're facing **"GLIBCXX_"** error after a successful compilation of the project, you can try to run this commands:

```
sudo add-apt-repository ppa:ubuntu-toolchain-r/test  
sudo apt-get update  
sudo apt-get install gcc-4.9  
sudo apt-get upgrade libstdc++6  
```
---  

[Next step]({{site.url}}{{site.baseurl}}/start/learn/quickstart/step2)
