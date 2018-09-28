---
author: jab
title: This Month in Pinball August 2018
tags: [this_month_in_pinball, MPF]
---
What happened in MPF-land in August 2018?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# Current Release 0.50

We released MPF 0.50.13 with bugfixes.

## Changes

None

## Bugfixes

* [Restore Diverter State After Ball Search](https://github.com/missionpinball/mpf/commit/7930fbc4691676edb87d5601245dd460e18562f0) - jab

## Documentation

* [Document how to cancel a show using flipper_cancel events](https://github.com/missionpinball/mpf-docs/commit/c060d879e61195dacb29c5dcd64a4a60810a32e5) - mwiz
* [Fix combo_switches syntax](https://github.com/missionpinball/mpf-docs/commit/721c6166b07e7dfd9b11ed53d46b9102be0fbfa5) - jab

# Dev release (future 0.51)

We pushed MPF dev-7.

## Changes

* [Improve performance without logging](https://github.com/missionpinball/mpf/commit/b870147b3031f4ab5cea90911269013b8d86f3ac) - jab
* [Add support for P3-Roc burst optos](https://github.com/missionpinball/mpf/commit/c98832f4e175a4cc2d1de0c546a3b9d65432aedb) - jab
* [Allow users to disable ball search rounds](https://github.com/missionpinball/mpf/commit/2ded24ac3076c877a53ed575205fe124378888e0) - jab
* [Define alignment for segment displays](https://github.com/missionpinball/mpf/issues/1201) - jab
* [Add restart_events to shots and shot groups](https://github.com/missionpinball/mpf/pull/1213) - avanwinkle
* [Add placeholder support to event_player](https://github.com/missionpinball/mpf/pull/1212) - avanwinkle


## Bugfixes

* [Fix debug flag in P-Roc and P3-Roc](https://github.com/missionpinball/mpf/commit/015fc4d8508ffadf9324100a5d9280dd4e781b49) - jab
* [Prevent achivements from enabling after restoring state](https://github.com/missionpinball/mpf/pull/1211) - avanwinkle
* [Fix ms vs sec in timer pause](https://github.com/missionpinball/mpf/pull/1214) - avanwinkle
* [Fix depreation warnings in kivy scale](https://github.com/missionpinball/mpf-mc/pull/343) - avanwinkle

## Documentation

* [Document how to cancel a show using flipper_cancel events](https://github.com/missionpinball/mpf-docs/commit/acb6c6ba2efaaba8b5a93e71f229772f8b6c96a9) - mwiz
* [Document wiring and voltages](https://github.com/missionpinball/mpf-docs/commit/a7a70a8b3c454f725edb5773fceadf77659f2584) - jab
* [Mode corrections](https://github.com/missionpinball/mpf-docs/pull/169) - mwseiden
* [Document electrical details of optos](https://github.com/missionpinball/mpf-docs/commit/7c06de742a730449b9d82e32a864b9fcfa3684d2) - jab
* [Update shot group profiles documentation](https://github.com/missionpinball/mpf-docs/pull/171) - avanwinkle
* [Document how to use player variables with counters](https://github.com/missionpinball/mpf-docs/pull/172) - mwseiden
* [Document appliance classes and common ground](https://github.com/missionpinball/mpf-docs/commit/44c15465db97108d93fad1637c43a3778afdd4aa) - jab
* [Added examples for PD-LED](https://github.com/missionpinball/mpf-docs/commit/a57ddb305abf8b4738e355143be1222d6c763b6b) - jab


Did we forget anything? Please let us know.

