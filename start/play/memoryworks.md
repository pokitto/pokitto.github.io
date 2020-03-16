---
title: Understand how Pokitto loads games
parent: Play
nav_order: 1
has_children: false
---

## How the game loader works

The game loader, <span style="font-weight:bold; color:lime" >**Kraken**</span> (by bl_ackrain), is a small piece of code that lives above the game program (like someone living in the attic of a house).

When you press 'C' (the smallest button in the front of Pokitto) during startup when prompted, the Pokitto processor jumps to the attic to the loader code.

In Kraken, after you have chosen the game you want to load, the loader copies that game from **SD card** into the **FLASH** memory below the loader. 

When Pokitto is restarted, it begins running the new game.


### Understanding Pokitto memory in detail

Pokitto has 4 kinds of memory, in order of size from smallest to largest:

1. 4kB of EEPROM memory
  - EEPROM memory is very small. It is used to store highscores and system settings
2. 36kB of RAM memory
  - RAM memory is the "working memory" of Pokitto, that is used for calculations when games are running
  - RAM memory is emptied every time device is switched off. It can not store data permanently
3. 256kB of FLASH memory
  - FLASH memory is where the actual program is running from
  - FLASH keeps the current program even when Pokitto is OFF
  - Every program needs to fit into the FLASH. Because the game loader also needs space, programs need to be 220kB or less
4. 2GB or bigger SD card (when comes with Pokitto)
  - SD card can hold as many games as you want and will fit on the SD card
  - SD card also has music and other data that is needed by the games
  - the loader gets games from the SD card and loads them into FLASH

