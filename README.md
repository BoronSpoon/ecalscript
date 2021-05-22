# ECal Script
markdown style easy online calculator description language   
ECal stands for Easy Calculator

## example
- script
  ```
  t V   n V   s V
  t I   n I   s I
  ---
  t R   n R   s R   b calc

  # t V = voltage; t I = current; t R = resistance
  # n V = 0; n I = 1; n R = 0
  # s V = [V]; s I = [A]; s R = [Ω]; b calc = calculate
  @ b calc -> n R = n V / n I
  ```
- display result
  - ![ui1.png]("pics/ui1.png?raw=true")

## syntax
- html part
  - `[t,n,s,b]_`(t,n,s,b followed by one space) denotes variable type
    - t: text
    - n: number
    - s: select
    - b: button
  - `___`(three spaces) denotes new column
  - `---` denotes section line
- script part
  - `#` denotes initial condition
  - `@ b button_name` denotes event at button press
  - `;`(semicolon) splits each expressions
