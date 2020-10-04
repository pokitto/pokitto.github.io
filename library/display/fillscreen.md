---
title: fillScreen
nav_order: 1
has_children: false
parent: Library Documentation Display
permalink: /library/display/fillscreen
---

## fillScreen(uint16_t color)

## Description
Fill the whole screen with the selected color index of the actual palette.


## Example

<div class="code-example" markdown="1">
**main.cpp**
</div>


```cpp
#include "Pokitto.h"

int color = 0;
void update() {
    using PD = Pokitto::Display;
    //fill all screen with one color
    PD::fillScreen((color / 10) % 16);
    color++;
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
    <img src="fillscreen.gif">
</div>
