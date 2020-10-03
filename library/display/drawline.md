---
title: drawLine
nav_order: 3
has_children: false
parent: Library Documentation
permalink: /library/display/drawline
---

How to draw a line.

## drawLine(x0, y0, x1, y1)

Draws a line of the current color (you can choose index color with ).

## Parameters

### x0
The x coordinate from where the line will start. 

### y0
The y coordinate from where the line will start. 

### x1
The x coordinate where the line will end.

### y1
The y coordinate where the line will end.

## Example

<div class="code-example" markdown="1">
**main.cpp**
</div>


```cpp
#include "Pokitto.h"
using PD = Pokitto::Display;

void init() {
}

void update() {
   PD::drawLine(0,0,42,42);
}
```
