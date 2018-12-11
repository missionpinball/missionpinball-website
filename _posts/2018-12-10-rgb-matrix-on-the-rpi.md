---
layout: post
author: jab
title: RGB Matrix on The Raspberry Pi
tags: [hardware, MPF]
---
We just upstreamed support for RGB Matrix devices connected to a Raspberry Pi.

Michael Betz, one of our fellow MPF users, build
[custom control boards](https://github.com/yetifrisstlama/Fan-Tas-Tic-platform)
which he implemented as
[external platform for MPF](https://github.com/missionpinball/mpf-demo-platform).
It works via I2C and looks
[like pretty cool homebrew project](https://yetifrisstlama.github.io/fan-tas-tic-firmware-upgrade/).
Make sure to check it out!
In addition to his control boards he also implemented support for
RGB Matrix devices connected to a Raspberry Pi which can be bought
at Adafruit, Sparkfun, ebay, aliexpress or various other places.
Those work using the
[python bindings](https://github.com/hzeller/rpi-rgb-led-matrix/tree/master/bindings/python#using-the-library)
of the excellent
[rpi-rgb-led-matrix library](https://github.com/hzeller/rpi-rgb-led-matrix)
by Henner Zeller.

We thank Michael for all his work and upstreamed the platform.
You can read our documentation about the
[RPi DMD](http://docs.missionpinball.org/en/dev/hardware/rpi_dmd/index.html)
and try it out today.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
