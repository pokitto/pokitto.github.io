---
title: API Reference
nav_order: 1
has_children: false
parent: Library Documentation
permalink: /library/reference
---

# PokittoLib API Reference

Here is listed and explained all Pokitto specific functions, part of the PokittoLib (see [Getting started]({{site.url}}{{site.baseurl}}/start/learn) to install it).

<h1> Pokitto <span class="label label-green">namespace</span></h1>

<h2> Core <span class="label label-purple">class</span></h2>

### Functions

| Name                                                                     | Description                                                  |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------|
| [begin()]({{site.url}}{{site.baseurl}}/library/core/begin)               | Initialize Pokitto.                                          | 
| [isRunning()]({{site.url}}{{site.baseurl}}/library/core/isrunning)       | Check run state.                                             |
| [update()]({{site.url}}{{site.baseurl}}/library/core/update)             | Update screen, buttons, sound.                               |
| [getTime()]({{site.url}}{{site.baseurl}}/library/core/gettime)           | Get value of time elapsed in milliseconds.                   |
| [getTime_us()]({{site.url}}{{site.baseurl}}/library/core/gettime_us)     | Get value of time elapsed in microseconds.                   |
| [wait()]({{site.url}}{{site.baseurl}}/library/core/wait)                 | Wait for n milliseconds.                                     |
| [jumpToLoader()]({{site.url}}{{site.baseurl}}/library/core/jumptoloader) | Call the loader.                                             |


<h2> Display <span class="label label-purple">class</span></h2>

### Functions

| Name                                                                                   | Description                                                  |
|:---------------------------------------------------------------------------------------|:-------------------------------------------------------------|
| [drawBitmap()]({{site.url}}{{site.baseurl}}/library/display/drawbitmap)                | Draw bitmap to the screen.                                   | 
| [drawPixel()]({{site.url}}{{site.baseurl}}/library/display/drawpixel)                  | Draw pixel to the screen.                                    |
| [getPixel()]({{site.url}}{{site.baseurl}}/library/display/getpixel)                    | Get pixel color.                                             |
| [fillScreen()]({{site.url}}{{site.baseurl}}/library/display/fillscreen)                | Fill the screen with the specified color.                    |
| [clear()]({{site.url}}{{site.baseurl}}/library/display/clear)                          | Clear the screen.                                            |
| [setInvisibleColor()]({{site.url}}{{site.baseurl}}/library/display/setinvisiblecolor)  | Set invisible color.                                         |
| [setColor()]({{site.url}}{{site.baseurl}}/library/display/setcolor)                    | Set color.                                                   |
| [getHeight()]({{site.url}}{{site.baseurl}}/library/display/getheight)                  | Get screen height.                                           |
| [getWidth()]({{site.url}}{{site.baseurl}}/library/display/getwidth)                    | Get screen width.                                            |
| [load565Palette()]({{site.url}}{{site.baseurl}}/library/display/load565palette)        | Load a 565 palette.                                          |
| [loadRGBPalette()]({{site.url}}{{site.baseurl}}/library/display/loadrgbpalette)        | Load a RGB palette.                                          |


<h2> Sound <span class="label label-purple">class</span></h2>

### Functions

| Name                                                                              | Description                                                  |
|:----------------------------------------------------------------------------------|:-------------------------------------------------------------|
| [playSFX()]({{site.url}}{{site.baseurl}}/library/sound/playsfx)                   | Play sound from internal flash.                              | 
| [playMusicStream()]({{site.url}}{{site.baseurl}}/library/sound/playmusicstream)   | Play sound file from the SD card.                            |
| [pauseMusicStream()]({{site.url}}{{site.baseurl}}/library/sound/pausemusicstream) | Pause sound file playback.                                   |
| [ampEnable()]({{site.url}}{{site.baseurl}}/library/sound/ampEnable)               | Enable/disable audio amplifier.                              |
| [ampIsoOn()]({{site.url}}{{site.baseurl}}/library/sound/ampIsOn)                  | Enable/disable audio amplifier.                              |
| [setVolume()]({{site.url}}{{site.baseurl}}/library/sound/setVolume)               | Set Volume.                                                  |
| [getVolume()]({{site.url}}{{site.baseurl}}/library/sound/setVolume)               | Get Volume.                                                  |

<h2> Buttons <span class="label label-purple">class</span></h2>

### Functions

| Name                                                                          | Description                                                      |
|:------------------------------------------------------------------------------|:-----------------------------------------------------------------|
| [pressed()]({{site.url}}{{site.baseurl}}/library/buttons/begin)               | Check if button pressed.                                         | 
| [released()]({{site.url}}{{site.baseurl}}/library/buttons/isrunning)          | Check if button released.                                        |
| [held()]({{site.url}}{{site.baseurl}}/library/buttons/update)                 | Check if button held for 'n' frmaes.                             |
| [repeat()]({{site.url}}{{site.baseurl}}/library/buttons/gettime)              | Returns true every 'period' frames when 'button' is held         |
| [timeHeld()]({{site.url}}{{site.baseurl}}/library/buttons/gettime_us)         | Get The number of frames during which the button has been held.  |
| [aBtn()]({{site.url}}{{site.baseurl}}/library/buttons/abtn)                   | Check if Button A pressed.                                       |
| [bBtn()]({{site.url}}{{site.baseurl}}/library/buttons/bbtn)                   | Check if Button B pressed.                                       |
| [cBtn()]({{site.url}}{{site.baseurl}}/library/buttons/cbtn)                   | Check if Button C pressed.                                       |
| [upBtn()]({{site.url}}{{site.baseurl}}/library/buttons/upbtn)                 | Check if Button up pressed.                                      |
| [downBtn()]({{site.url}}{{site.baseurl}}/library/buttons/downbtn)             | Check if Button down pressed.                                    |
| [rightBtn()]({{site.url}}{{site.baseurl}}/library/buttons/rightbtn)           | Check if Button right pressed.                                   |
| [leftBtn()]({{site.url}}{{site.baseurl}}/library/buttons/leftbtn)             | Check if Button left pressed.                                    |
| [aReleased()]({{site.url}}{{site.baseurl}}/library/buttons/areleased)         | Check if Button A released.                                      |
| [bReleased()]({{site.url}}{{site.baseurl}}/library/buttons/breleased)         | Check if Button B released.                                      |
| [cReleased()]({{site.url}}{{site.baseurl}}/library/buttons/creleased)         | Check if Button C released.                                      |
| [upReleased()]({{site.url}}{{site.baseurl}}/library/buttons/upreleased)       | Check if Button up released.                                     |
| [downReleased()]({{site.url}}{{site.baseurl}}/library/buttons/downreleased)   | Check if Button down released.                                   |
| [rightReleased()]({{site.url}}{{site.baseurl}}/library/buttons/rightreleased) | Check if Button right released.                                  |
| [leftReleased()]({{site.url}}{{site.baseurl}}/library/buttons/leftreleased)   | Check if Button left released.                                   |
| [aHeld()]({{site.url}}{{site.baseurl}}/library/buttons/aheld)                 | Check if Button A held for 'n' frames.                           |
| [bHeld()]({{site.url}}{{site.baseurl}}/library/buttons/bheld)                 | Check if Button B held for 'n' frames.                           |
| [cHeld()]({{site.url}}{{site.baseurl}}/library/buttons/cheld)                 | Check if Button C held for 'n' frames.                           |
| [upHeld()]({{site.url}}{{site.baseurl}}/library/buttons/upheld)               | Check if Button up held for 'n' frames.                          |
| [downHeld()]({{site.url}}{{site.baseurl}}/library/buttons/downheld)           | Check if Button down held for 'n' frames.                        |
| [rightHeld()]({{site.url}}{{site.baseurl}}/library/buttons/rightheld)         | Check if Button right held for 'n' frames.                       |
| [leftHeld()]({{site.url}}{{site.baseurl}}/library/buttons/leftheld)           | Check if Button left held for 'n' frames.                        |

