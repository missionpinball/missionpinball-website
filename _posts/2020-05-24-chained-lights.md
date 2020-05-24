---
layout: post
author: jab
title: Chained Lights in MPF
tags: [MPF, lights]
---
Configuring a lot of lights in your machine is often tedious and error-prone.
Especially, if you are using serial LEDs where you know that a light is
physically localed after the previous one.
What if we could exploit this property in config? 

Instead of this:
```
lights:
  l_led0:
    channels:
      red:
        - number: 8-0
      green:
        - number: 8-1
      blue:
        - number: 8-2
  l_led1:
    channels:
      red:
        - number: 8-3
      green:
        - number: 8-4
      blue:
        - number: 8-5
      white:
        - number: 8-6
  l_led2:
    channels:
      red:
        - number: 8-7
      green:
        - number: 8-8
      blue:
        - number: 8-9
      white:
        - number: 8-10
```

You can now use (in MPF 0.54/dev):
```
lights:
  led_0:
    start_channel: 8-0
    subtype: led
    type: rgb    # will use red: 8-0, green: 8-1, blue: 8-2
  led_1:
    previous: led_0
    subtype: led
    type: rgbw   # will use red: 8-3, green: 8-4, blue: 8-5, white: 8-6
  led_2:
    previous: led_1
    subtype: led
    type: rgbw   # will use red: 8-7, green: 8-8, blue: 8-9, white: 8-10
```

This saves a lot of typing for RGBW LEDs.
It also works for parallel LEDs.
For instance, you might want to define the first light number per board and
then define all subsequent lights on that board using the new syntax.
This would allow you to easily change the board number for all light at once.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
