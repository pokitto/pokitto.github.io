---
title: drawPixel
nav_order: 1
has_children: false
parent: Library Documentation Display
permalink: /library/display/drawpixel
---

## drawPixel(int16_t x, int16_t y)

## drawPixel(int16_t x, int16_t y, uint8_t color)

## Description
Draw a single point (pixel) in the screen specific coordinate using current color (you can choose index color with [setColor]({{site.url}}{{site.baseurl}}/library/display/setcolor))
or using the function call with color as parameter.

## Parameters

### x
The x coordinate where draw the pixel. 

### y
The y coordinate where draw the pixel.

### color
The color that will be used to draw the pixel, in case you don't want to set it with [setColor]({{site.url}}{{site.baseurl}}/library/display/setcolor)).


## Example

<div class="code-example" markdown="1">
**main.cpp**
</div>


```cpp
#include "Pokitto.h"

uint8_t i = 0;

void update() {
    using PD = Pokitto::Display;

    for (int x = 0; x < PD::width; x++) {
        for (int y = 0; y < PD::height; y++) {
            PD::drawPixel(x, y, ((x * y) / i) % 16); //draw pixel at x and y with a color
        }
    }
    i++;
}
```

Project settings
<div class="code-example" markdown="1">
**My_settings.h**
</div>

```
#define PROJ_SCREENMODE MODE15
```

<div style="min-width: 33.33%">
    <img src="drawpixel.gif">
</div>
