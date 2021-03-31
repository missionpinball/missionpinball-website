---
layout: post
author: jab
title: Preventing Flipper Overheating - Repulsing flippers when EOS opens
tags: [MPF, Flipper, Hardware]
---
MPF 0.55 support repulsing flippers when the EOS to counter knockdowns by fast
balls which sometimes happens during play.
This means PWM power on the flipper coil resulting in less heat and stronger
flippers.

Modern machines use
[pulse-width modulation (PWM)](https://en.wikipedia.org/wiki/Pulse-width_modulation)
to keep flipper bats up because most coils will
instantly burst into flames if you enable them at 48V which are typically used
in today's machines.
PWM uses a so called duty-cycle which determines how much energy moves into
the flippers.
More energy strictly results in more power but that energy also turns into
heat.
Unfortunately, the resistance in copper wires in the coil increases with the
temperature and, consequently, the less current and energy will flow through
the coil.
As a result the coil will become weaker of time when it heats up.
Since we do not know the temperature in software this cannot easily be
compensated as runtime (and the coil would probably become even hotter and burn
if we would try). 

Finding the right spot where the coil is strong enough, knockdowns do not
happen and the temperature stays low enough is not generally easy.
Parts age over time, environment temperature differs between location and
even the voltage might fluctuate.
We have seen overheating of coils in some machines by newer manufacturers.

So what can we do about this?
We can detect when the EOS switch opens while the flipper button is active
and repulse the flipper coil.
Ideally, this should happen inside the pinball hardware but this is currently
only supported in Stern Spike 1/2 (out of the platforms supported in MPF).
For all remaining platforms, we mitigate this in software in MPF.
This introduces a few milliseconds of delay but it should be fast enough that
the player does not notice it.

This is how you can enable it in MPF:

```yaml
flippers:
    single_wound_flipper:
        main_coil: c_flipper_single_main
        activation_switch: s_flipper_single
        eos_switch: s_flipper_single_eos
        use_eos: true
        repulse_on_eos_open: true
        eos_active_ms_before_repulse: 500
    dual_wound_flipper:
        main_coil: c_flipper_dual_wound_main
        hold_coil: c_flipper_dual_wound_hold
        activation_switch: s_flipper_dual_wound
        eos_switch: s_flipper_dual_wound_eos
        use_eos: true
        repulse_on_eos_open: true
        eos_active_ms_before_repulse: 500
```

To prevent repeated activations MPF will wait `eos_active_ms_before_repulse` ms
before a repulse can happen.
There are certain races between hardware rules and this mechanism which MPF
tries to handle (but we might have missed cases - let us know if you find any
rough edges or weird behaviour with this).

In general, this should allow you to reduce PWM power by a lot and instead
use repulses in the rare case of knockdowns.
This should work with all platforms and will use hardware rules if your
platform supports them.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
