# ECal Script
markdown style easy online calculator description language   
ECal stands for Easy Calculator

## example
```
t voltage   n voltage   s voltage
t current   n current   s current
---
t resistance   n resistance   b calculate
# n voltage = 0; n current = 1; n resistance = 0
@ b calculate -> n resistance = n voltage / n current
```

## syntax
- html part
  - `[t,n,s,b] `(t,n,s,b followed by one space) denotes variable type
    - t: text
    - n: number
    - s: select
    - b: button
  - `   `(three spaces) denotes new column
  - `---` denotes section line
- script part
  - `#` denotes initial condition
  - `@ b button_name` denotes event at button press
  - `;`(semicolon) splits each expressions
