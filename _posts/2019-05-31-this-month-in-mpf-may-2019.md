---
layout: post
author: jab
title: This Month in MPF May 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in May 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* We added hardware platforms to the [MPF Projects List](https://missionpinball.org/projects.html). Please have a look if we got it right for your machine (or let us know if it is missing).
* [Want to meet us?]({% post_url 2019-05-18-want-to-meet-us %}) - jab
* [Virtual Pinball (VPX) support]({% post_url 2019-05-25-virtual-pinball-and-mpf %}) - mfuegemann


# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [ESCAPE!]({% link _projects/escape.md %})
* [Zelda]({% link _projects/zelda.md %})
* [Mass Effect]({% link _projects/mass_effect.md %})
* [Archer]({% link _projects/archer.md %})
* [Greek Gods]({% link _projects/greek_gods.md %})
* [Genie]({% link _projects/genie.md %})

We know that there are a lot more projects. Let us know if you want to be listed here as well (it does not matter in which stage your project is).

# 0.52 release

We released MPF 0.52.2 and MPF-MC 0.52.1.

## Changes

* No changes

## Bugfixes

* No changes

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev20 and MPF-MC 0.53.0-dev0.

## Changes/New features

* [Allow newer FAST firmware versions](https://github.com/missionpinball/mpf/pull/1356) - jab based on problems with Firmware 1.05 by Brian Cox
* [Support inverted switches and non-numeric drivers in Virtual Pinball](https://github.com/missionpinball/mpf/pull/1360) - mfuegemann
* [Extend README and add hardware rules to VPX Bridge](https://github.com/missionpinball/mpf-vpcom-bridge/pull/1) and [Test](https://github.com/missionpinball/mpf-vpcom-bridge/pull/2)- mfuegemann
* [Placeholders in credits mode](https://github.com/missionpinball/mpf/pull/1357) - jab
* [Placeholders in tilt mode](https://github.com/missionpinball/mpf/pull/1358) - jab
* [RGB LEDs and flashers in Virtal Pinball](https://github.com/missionpinball/mpf/pull/1363) - mfuegemann
* [Update asciimatics](https://github.com/missionpinball/mpf/pull/1362) - jab
* [Add --vpx commandline option to mpf](https://github.com/missionpinball/mpf/pull/1364) and [mc](https://github.com/missionpinball/mpf-mc/pull/373)- jab
* [Add VPX demo table with MPF config](https://github.com/missionpinball/mpf-vpcom-bridge/pull/3) - mfuegemann
* [Placeholders for StateMachine devices](https://github.com/missionpinball/mpf/pull/1365) - jab
* [Initial support for the Arduino Pinball Platform](https://github.com/missionpinball/mpf/commit/0021aa4c80c3f5c4db02c7ed0e797f0f2419340e) - jab, bontango and blackknight
* [More debug in FAST platform](https://github.com/missionpinball/mpf/commit/c79a36b312d33c5cc546e4d9637f51ccef3ddcaf) and [longer wait times](https://github.com/missionpinball/mpf/commit/e031cb047dcecaaeb9eb37fc11422ea657e2ed71) - jab to support more FAST firmwares
* [Generic System 11 A/C Relay handling (for APC and Snux)](https://github.com/missionpinball/mpf/pull/1370) - jab
* [Improve duplicate event handler message](https://github.com/missionpinball/mpf/commit/bebf593f97b068f07b3af69e93f48b3c8e595974) - jab as it [caused confusion for Sepp](https://groups.google.com/forum/#!topic/mpf-users/epVKlaU9Yo8)
* [Better error message when number is empty]() - jab based on [report by Sepp](https://groups.google.com/forum/#!msg/mpf-users/oHsUeEJr2yI/Y1hg21iNBAAJ) 
* [Placeholders in show_tokens in show_player](https://github.com/missionpinball/mpf/pull/1379) - jab to [allow dynamic values in all widgets](https://groups.google.com/forum/#!topic/mpf-users/lUd6Z2lU_eo)
* [More useful and accurate validation errors in dicts](https://github.com/missionpinball/mpf/commit/240c4f9faabd58b8e96b3509b9a7d28ad0fc13fc) - jab

## Bugfixes

* [Prevent shutdown glitches in FAST](https://github.com/missionpinball/mpf/commit/90acd6c60da1c0b4a4922edbeaca247228a54d41) - jab with the help of Dave
* [Prevent crash during early errors in P-Roc](https://github.com/missionpinball/mpf/commit/95ac7c6eb8cd60712fa1c3cad557fcd9ffaa529a) - jab based on report by Coleman
* [Preserve curly brakets in string_to_list](https://github.com/missionpinball/mpf/pull/1361) - avanwinkle
* [Fix bug preventing access to settings in custom code](https://github.com/missionpinball/mpf/pull/1369) - avanwinkle
* [Properly implement disable_random event in random_event_player](https://github.com/missionpinball/mpf/pull/1374) - avanwinkle
* [Fix enable attribute for placeholders in devices](https://github.com/missionpinball/mpf/pull/1372) - avanwinkle

## Documentation

* [How to use virtual env on Mac with Kivy](https://github.com/missionpinball/mpf/pull/1355) - driskel
* [Improve dynamic values example](https://github.com/missionpinball/mpf-docs/pull/223) - MarkInc666
* [How to add credits settings to service mode](https://github.com/missionpinball/mpf-docs/commit/744f29f861a243d9e6c95a9d81aa56fa7f32feec) - jab
* [How to add tilt settings to service mode](https://github.com/missionpinball/mpf-docs/commit/8e05a161cfc21141a1e961f2a65ad8fa5b214d4c) - jab
* [Document placeholders for StateMachine devices](https://github.com/missionpinball/mpf-docs/pull/224) - jab
* [Document state machine configs](https://github.com/missionpinball/mpf-docs/commit/aadea2392c08c0d79ee96a8bc23b4d6639f6ae5e) - jab
* [Add more config links and document timer transitions](https://github.com/missionpinball/mpf-docs/commit/e797a5fc8457d521bfd4263908a0c226171ff2f7) - jab
* [Fixes in the tutorial](https://github.com/missionpinball/mpf-docs/pull/227) and [more](https://github.com/missionpinball/mpf-docs/pull/228) - ironspider
* [Document LISY protocol](https://github.com/missionpinball/mpf-docs/commit/cbb65ff49253befb1fb116d8d72d2f67a945f090) - jab
* [Update example links](https://github.com/missionpinball/mpf-docs/commit/8e0f5334f6df40733810c2627e71fc0db063808b) - GabeKnuth
* [Fix Mac install instructions](https://github.com/missionpinball/mpf-docs/commit/8016c8daf9c83ba2dafcde5ffef1244a02219a69) - GabeKnuth
* [Typos](https://github.com/missionpinball/mpf-docs/pull/232), [Bad English](https://github.com/missionpinball/mpf-docs/pull/230) and [more](https://github.com/missionpinball/mpf-docs/pull/229) - ironspider
* [Rotation is counter-clock wise not clockwise](https://github.com/missionpinball/mpf-docs/pull/231) - colemanomartin
* [Document game variables](https://github.com/missionpinball/mpf-docs/pull/233) - cfbenn
* [Improve tutorial](https://github.com/missionpinball/mpf-docs/pull/235) and [fix typos](https://github.com/missionpinball/mpf-docs/pull/236) - soraxxo

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen
* [Add control events to counters](https://github.com/missionpinball/mpf/pull/1342) - dziedada

## Upcoming changes

* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab
* [Full support for LISY35](https://github.com/missionpinball/mpf/issues/1218) - jab and bontango
* [Support for the APC platform](https://github.com/missionpinball/mpf/issues/1345) - jab, bontango and blackknight

## Do you want to contribute?

A list of things where we would love contributions (not exclusive):

* Pictures for the following devices: [pop bumpers](http://docs.missionpinball.org/en/dev/mechs/pop_bumpers/index.html),
  [incandescant bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/matrix_lights.html),
  [GI bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [GI LEDs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [data east optos](http://docs.missionpinball.org/en/dev/mechs/switches/optos.html),
  [dual wound coils](http://docs.missionpinball.org/en/dev/mechs/coils/dual_wound_coils.html),
  [coils](http://docs.missionpinball.org/en/dev/mechs/coils/index.html),
  [orbits](http://docs.missionpinball.org/en/dev/mechs/loops/index.html),
  [kickbacks](http://docs.missionpinball.org/en/dev/mechs/kickbacks/index.html),
  [kicking targets](http://docs.missionpinball.org/en/dev/mechs/targets/kicking_targets/index.html),
  [accelerometer](http://docs.missionpinball.org/en/dev/mechs/accelerometers/index.html),
  [playfield](http://docs.missionpinball.org/en/dev/mechs/playfields/index.html),
  [flashers](http://docs.missionpinball.org/en/dev/mechs/lights/flashers.html),
  [flippers](http://docs.missionpinball.org/en/dev/mechs/flippers/index.html),
  [score reels](http://docs.missionpinball.org/en/dev/mechs/score_reels/index.html),
  [diverters](http://docs.missionpinball.org/en/dev/mechs/diverters/index.html),
  [trough with optos](http://docs.missionpinball.org/en/dev/mechs/troughs/index.html) - please only send us picture where the rights belong to you
* Document asset pools such as [video_pools](http://docs.missionpinball.org/en/dev/config/video_pools.html), [image_pools](http://docs.missionpinball.org/en/dev/config/image_pools.html) or [show_pools](http://docs.missionpinball.org/en/dev/config/show_pools.html)
* [Create an electronical drawing for mechanical switches in matrix and on direct inputs](http://docs.missionpinball.org/en/dev/mechs/switches/mechanical_switches.html)
* [Document motors](http://docs.missionpinball.org/en/dev/mechs/motors/index.html)
* [Add an example or howto for timed switches](http://docs.missionpinball.org/en/dev/game_logic/timed_switches/index.html)
* [Add an example or howto for ball holds](http://docs.missionpinball.org/en/dev/game_logic/ball_holds/index.html)
* [Add an example or howto for combo switches](http://docs.missionpinball.org/en/dev/game_logic/combo_switches/index.html)
* [Add an example or howto for diverters](http://docs.missionpinball.org/en/dev/mechs/diverters/index.html)
* [Adding more devices to the built-in service mode](https://github.com/missionpinball/mpf/issues/693)
* [Good first issues in MPF](https://github.com/missionpinball/mpf/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
* [Good first issues in MPF-MC](https://github.com/missionpinball/mpf-mc/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
* [Good first issues in MPF-Monitor](https://github.com/missionpinball/mpf-monitor/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
* [More TODOs in the documentation](http://docs.missionpinball.org/en/dev/search.html?q=help_us_to_write_it&check_keywords=yes&area=default)

Other contributions are welcome as well.
Those are meant as starting point.
Let us know in the [forum](https://groups.google.com/forum/#!forum/mpf-users)
if you want to work on something or got questions.

## New contributors

Welcome driskel, mfuegemann, ironspider and soraxxo.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
