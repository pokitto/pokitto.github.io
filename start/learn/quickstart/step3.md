---
title: Upload a program to Pokitto
has_children: false
permalink: /start/learn/quickstart/step3
parent: Quick Start Guide
nav_order: 3
---

# Step 3: Upload a program to Pokitto

In this step we are going to flash the Pokitto HW with the binary file we created in the previous step.

## Linux (Ubuntu)

1. Put Pokitto in the flashing mode. The video in the end of the page shows how to do it (from the start of the video to 4:47). Just do not download the binary as instructed in the video, as we are going to use our own.  

2. If you installed Femto IDE under the "$HOME/bin/FemtoIDE" folder, open the terminal in the folder: "$HOME/bin/FemtoIDE/project/MyHello"

3. Copy the binary file to the flashing drive like below and wait for 5 seconds:
`dd bs=1024 conv=nocreat,notrunc if=MyHello.bin of=/media/$USER/CRP\ DISABLD/firmware.bin`

4. Power off and on Pokitto. Press A until you see the game screen. 

## Windows

1. Put Pokitto in the flashing mode. The video in the end of the page shows how to do it (from the start of the video to 4:47). Just do not download the binary as instructed in the video, as we are going to use our own.  

2. If you installed Femto IDE under the "C:\bin\FemtoIDE" folder, use the file manager to copy the file "C:\bin\FemtoIDE\project\MyHello\MyHello.bin" to the "CRP DISABLD" drive. You can replace the current file in the "CRP DISABLD" drive.

3. Power off and on Pokitto. Press A until you see the game screen. 

## Video of how to flash a binary to Pokitto in Windows. 

The USB cable connection and buttons apply for all OS’s:
<iframe width="560" height="315" src="https://www.youtube.com/embed/PKlNyBJP9GA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Finally!

If everything went properly you should come up with something like this:

![hello world](/assets/images/learn/hellopokitto.jpg)
