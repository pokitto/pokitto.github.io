---
title: Make your first program
has_children: false
permalink: /start/learn/quickstart/step2
parent: Quick Start Guide
nav_order: 2
---

# Step 2: Make your first program "Hello World!"
This program print a simple text "Hello World!" on your pokitto display. <b/>
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

[Next step]({{site.url}}{{site.baseurl}}/start/learn/quickstart/step3)
