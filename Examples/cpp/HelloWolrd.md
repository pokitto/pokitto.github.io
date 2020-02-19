---
title: Hello World
parent: C++
nav_order: 1
has_children: false
---


## Hello World
Your first program on the pokitto 
 
<div class="code-example" markdown="1">
**main.cpp**
</div>

```cpp
#include "Pokitto.h"
int main(){
    using PC=Pokitto::Core;
    using PD=Pokitto::Display;
    PC::begin();
    while( PC::isRunning() ){
        if( !PC::update() ) 
            continue;
        PD::print("hello world");
    }
    return 0;
}
```

<div class="code-example" markdown="1">
**My_settings.h**
</div>

```cpp
#define PROJ_SCREENMODE   MODE_HI_4COLOR
```