---
title: White Screen of Death!
parent: Play
nav_order: 2
has_children: false
---


## I only get a white screen!! Is my Pokitto broken?!

Relax. When a Pokitto is showing a white screen, it only means that the program that is now in its memory is somehow broken. You need to flash any valid Pokitto .bin binary file 

- download **start.bin** from [here](https://talk.pokitto.com/t/testing-loader-test-program-for-pokitto/508)

You do not need a MicroSD card, you only need the .bin binary

- then use [Method 2 (USB cable)](loading.md) to reflash Pokitto 



### Technical explanation of the "White Screen of Death"

The white screen of death is not a screen of death at all. It means that the internal chip ROM startup routine has detected a broken program in the internal flash memory of Pokitto. This can happen for many reasons, maybe the binary you are trying to use is  simply not a valid program or maybe your powered off or reset Pokitto while it was in progress of loading a game from the microSD card.

When the internal ROM check fails to find a valid program, it puts Pokitto AUTOMATICALLY into "reflash" mode ... and that mode gives the "white screen". Pokitto is not dead, it is just waiting for you to put a valid program in!

![Image](pokitto_whitescreen.png){: width="600px"}

