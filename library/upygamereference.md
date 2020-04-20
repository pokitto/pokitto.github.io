---
title: uPyGame Reference
nav_order: 1
has_children: true
parent: Library Documentation
permalink: /library/upygamereference
---

# Python uPyGame API Reference

Here is listed and explained all Pokitto specific MicroPython functions, part of the uPyGame library.

<h1> uPyGame <span class="label label-green">namespace</span></h1>

<h2> TAS <span class="label label-purple">class</span></h2>

The bufferless TAS ("Tiles And Sprites") modes are somewhat limited, but give more free memory (up to 3 KB more). The TAS modes are:
* HighRes TAS mode (220x176, 16 colors)
* LowRes TAS mode (110x88, 16 colors)

With the TAS mode you can only draw tiles or sprites (e.g. bitmaps) to the screen. Any graphics primitive drawing functions, like a line or a circle, will not work. Also the normal text drawing is limited as each character takes one sprite (!). The TAS modes has separate settings for the tile size (default: 16x16 pixel) and maximum sprite and character count (default: 100).

These are the only normal drawing functions you can use in the TAS mode:
* Tilemap.draw()
* Surface.Blit() (limited to certain bitmap width and height, and bitmap count)
* draw.Text() (limited to certain character count per screen. Use TAS UI methods instead if possible.)

The TAS mode has 3 layers which are draw in the following order, from back to front:
1. The background tilemap layer
2. The sprite layer i.e. everything that is drawn with Surface.Blit())
3. The TAS UI tilemap layer. That is a tilemap that covers the whole screen. The tile size is 6x6 pixels.

The TAS UI API is used for drawing text and UI controls on the TAS mode. TAS UI methods use always the color indices 1-3 for the UI elements. The following TAS UI class could be used to draw to the frontmost layer.

### Functions

| Name                                                                     | Description                                                  |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------|
| [setCursor()]({{site.url}}{{site.baseurl}}/library/upygame/setcursor)               | Set the cursor position.                                          | 
| [printString()]({{site.url}}{{site.baseurl}}/library/upygame/printstring)       | Print a text.                                             |
| [printInteger()]({{site.url}}{{site.baseurl}}/library/upygame/printinteger)             | Print an integer number.                               |
| [clear()]({{site.url}}{{site.baseurl}}/library/upygame/clear)     | Clear all UI tiles, i.e. all text and graphics.                   |
| [setTile()]({{site.url}}{{site.baseurl}}/library/upygame/settile)           | Set the content of a tile.                   |
| [fillRectTiles()]({{site.url}}{{site.baseurl}}/library/upygame/fillrecttiles)                 | Fill the rectangular are of tile with a tile content.                                     |
| [drawBox()]({{site.url}}{{site.baseurl}}/library/upygame/drawbox) | Draw a box with borders.                                             |
| [drawGauge()]({{site.url}}{{site.baseurl}}/library/upygame/drawgauge) | Draw a gauge.                                             |

### Constants

| Name                                                                     | Description                                                  |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------|
| EMPTY_TILE               | A tile id. The lower layers are showing through if the tile is empty.                                          | 
| RIGHT_ARROW_TILE       | A tile id. A right arrow tile can be used e.g. in menu items to indicate focus.                                             |
| LEFT_ARROW_TILE             | A tile id. A left arrow tile can be used e.g. in menu items to indicate focus.                               |
| UP_ARROW_TILE     | A tile id for an up arrow tile.                   |
| DOWN_ARROW_TILE           | A tile id for a down arrow tile.                   |
| UNCHECKED_TILE                 | A tile id for the unchecked mark for the checkbox.                                     |
| CHECKED_TILE | A tile id for the checked mark for the checkbox.                                             |
| SPACE_TILE | A tile id. TAS UI background color is used for the space tile.                                             |


<h2> Other classes  TODO <span class="label label-purple">class</span></h2>

