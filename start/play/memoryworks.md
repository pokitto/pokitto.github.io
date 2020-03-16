---
title: Understand how Pokitto loads games
parent: Play
nav_order: 1
has_children: false
---

## Pokitto has many types of memory

Pokitto has 4 kinds of memory, in order of size from smallest to largest:
1. 4kB of <span style="background-color:#00AA00; color:black" >EEPROM</span> memory
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

### How the game loader works

Work in progresss....


1. Download and extract zip package
2. Put Pokitto in flash programming mode (shows as CRP_DISABLD flash drive)
3. Delete `firmware.bin` on Pokitto flash drive


<p class="fs-3 text-yellow-300">
* <strong>Attention: put only 1 of the .bin files on the Pokitto</strong> (the flash drive called CRP_DISABLD). This will install the SD loader into the memory. Put all of the unzipped .bin files on the SD card. Then you can swap games using the loader. In other words: do not try to put all of the binary files on the Pokitto at once, they will not fit!
</p>
