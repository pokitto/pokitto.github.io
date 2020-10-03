---
title: Hello World New
parent: C++
nav_order: 2
has_children: false
permalink: /examples/cpp/helloworldnew
---


## Hello World
Your first program on the pokitto in a simpler way
 
<div class="code-example" markdown="1">
**main.cpp**
</div>

```cpp
#include "Pokitto.h"

void init() {
    //Here put any code you want to execute at startup
}

void update() {
    //This should be executed at the required FPS
    using PD = Pokitto::Display;
    PD::print("hello world");
}
```