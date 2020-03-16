---
title: Understand how Pokitto loads games
parent: Play
nav_order: 1
has_children: false
---

WIP

## How Pokitto loads games

Pokitto has 4 kinds of memory, in order of size from smallest to largest:
1. 4kB of EEPROM memory
2. 36kB of RAM memory
3. 256kB of FLASH memory
4. 2GB or bigger SD card (when comes with Pokitto) 

EEPROM memory is very small. It is used to store highscores and system settings.


You will find a Ready-made disk of Pokitto games here:
> [Latest Game Disk and Game Loader](https://www.pokitto.com/games/)


### Instructions
1. Download and extract zip package
2. Put Pokitto in flash programming mode (shows as CRP_DISABLD flash drive)
3. Delete `firmware.bin` on Pokitto flash drive


<p class="fs-3 text-yellow-300">
* <strong>Attention: put only 1 of the .bin files on the Pokitto</strong> (the flash drive called CRP_DISABLD). This will install the SD loader into the memory. Put all of the unzipped .bin files on the SD card. Then you can swap games using the loader. In other words: do not try to put all of the binary files on the Pokitto at once, they will not fit!
</p>
