---
layout: post
author: jab
title: StepStick Steppers in MPF
tags: [hardware, MPF]
---
StepStick Stepper Controllers in MPF

We added support for simple inexpensive stepper controllers such as the
[StepStick](https://reprap.org/wiki/StepStick),
[DRV8825](https://www.pololu.com/product/2133) and various clones.
Those are readily available at Pololu, Adafruit, Sparkfun, Amazon, ebay,
Aliexpress and other electronics outlets.
The StepStick supports a simple two or three output interface
(direction, step and optional enable) which should work on almost any
pinball controller or via generic GPIOs (on the [RPi](https://docs.missionpinball.org/en/dev/hardware/rpi/index.html) or
[P3-Roc](https://docs.missionpinball.org/en/dev/hardware/multimorphic/switches_p3_roc.html#burst-switches-as-local-inputs)).
The number of steps per second might be a bit limited but enough for
most applications in pinball machines.
See the [StepStick documentation](https://docs.missionpinball.org/en/dev/hardware/stepstick/index.html)
for details.
MPF also supports [more advanced stepper controllers](https://docs.missionpinball.org/en/dev/hardware/stepper_platforms.html)
in case you need advanced features.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
