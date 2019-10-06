---
layout: post
author: jab
title: This Month in MPF August 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in August 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* Want to participate in Hacktoberfest 2019? Consider [contributing MPF](http://docs.missionpinball.org/en/dev/about/contributing_to_mpf.html) or the [MPF documentation](http://docs.missionpinball.org/en/dev/about/contributing_to_mpf_docs.html).

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Mindcrime]({% link _projects/mindcrime.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anthing wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.52 release

We released MPF 0.52.3 and MPF-MC 0.52.5.

## Changes

* No changes

## Bugfixes

* No changes

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev55 and MPF-MC 0.53.0-dev5.

## Changes/New features

* [Move code out of the hot path for light updates](https://github.com/missionpinball/mpf/pull/1397) - jab
* [Reserve all show_player options in show_tokens to prevent indent mistakes](https://github.com/missionpinball/mpf/pull/1399) - jab based on [bug report by Alex](https://groups.google.com/forum/#!topic/mpf-users/J0UBP81ppfg)
* [Improve linter and remove previously undetected unused imports](https://github.com/missionpinball/mpf/pull/1400) - jab
* [Better debug output for LISY platform](https://github.com/missionpinball/mpf/commit/b28c83fdcf860a3da90e3791d6ae82e1211db1b2) - jab
* [Fix segment display mapping for APC](https://github.com/missionpinball/mpf/commit/d8232883fc614177b188bc33f6794bc1fb72ce81) - jab
* [Configuration setting for player_vars and machine_vars to show in text ui](https://github.com/missionpinball/mpf/pull/1406) - avanwinkle
* [Better command logging for the P/P3-Roc](https://github.com/missionpinball/mpf/commit/163e769fa63bc745ffecce1497458942339212e6) - jab


## Bugfixes

* [Fixes for latest Spike Firmware](https://github.com/missionpinball/mpf/commit/f235b9a70f8d81d38e4e77c0571690aef7bd35b0) and [bridge](https://github.com/missionpinball/mpf-spike/commit/dde2bd367e7dcbdc84e5e7433e900dee4f652810) - jab
* [Always send a multiple of three LEDs to the Fadecandy to fix RGBW](https://github.com/missionpinball/mpf/commit/bae40db64e1496506f44596d24b58dbe85241b09) - jab based on [bug report by Cadrion](https://groups.google.com/forum/#!topic/mpf-users/inJzJVlWVWU)
* [Fix polarity issue on P-Roc with WPC hardware](https://github.com/missionpinball/mpf/commit/2aafe828656d09921e959f4c2f0208ac70f6a23e) - jab
* [LISY command fixes in protocol v0.9](https://github.com/missionpinball/mpf/commit/3bf547d0bf18005b56a1387b73cae013cd9d8774) and [2](https://github.com/missionpinball/mpf/commit/3058fc6c599ca2db8cd088520327493160480752) - jab
* [Fix image unload crash in MC](https://github.com/missionpinball/mpf-mc/pull/384) - avanwinkle

## Documentation

* [Document modes in subfolders](https://github.com/missionpinball/mpf-docs/pull/249) - pmansukhani
* [Wording improvments](https://github.com/missionpinball/mpf-docs/pull/250), [grammar fixes](https://github.com/missionpinball/mpf-docs/pull/253), [typos](https://github.com/missionpinball/mpf-docs/pull/254), [more typos](https://github.com/missionpinball/mpf-docs/pull/255), [more grammar](https://github.com/missionpinball/mpf-docs/pull/256), [simple past](https://github.com/missionpinball/mpf-docs/pull/257), [proper count](https://github.com/missionpinball/mpf-docs/pull/259) - ironspider (a lot of fixes)
* [More precise description](https://github.com/missionpinball/mpf-docs/pull/258) - ironspider
* [Add modern Stern Opto Trough](https://github.com/missionpinball/mpf-docs/pull/251) - ironspider
* [Fix segment_displays in shows](https://github.com/missionpinball/mpf-docs/pull/252) - snux
* [Document LISY35 flipper enable](https://github.com/missionpinball/mpf-docs/commit/8472924c3d19eca3079e62ac24f32db865cca31d) - jab based on [question by Dave](https://groups.google.com/forum/#!topic/mpf-users/bHj-Tvh2KhY)
* [Document local outputs on the P-Roc when using PDB boards](https://github.com/missionpinball/mpf-docs/commit/e3e83bc19ebb6ffa314560c3d05a7cd2dad63e3b) - jab
* [Update LISY procotol](https://github.com/missionpinball/mpf-docs/commit/8ff96dd5ece1e8112079f814b645d3a56691adca) - jab

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen

## Upcoming changes

* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab
* [Full support for LISY35](https://github.com/missionpinball/mpf/issues/1218) - jab and bontango

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
* [More TODOs in the documentation](http://docs.missionpinball.org/en/dev/search.html?q="Help+us+to+write+it"&check_keywords=yes&area=default)

Other contributions are welcome as well.
Those are meant as starting point.
Let us know in the [forum](https://groups.google.com/forum/#!forum/mpf-users)
if you want to work on something or got questions.

## New contributors

Welcome .

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
