---
layout: post
author: jab
title: This Month in MPF Dezember 2018
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in Dezember 2018?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* We created a list of [publicly documented projects by MPF users on our website]({% link projects.html %}).

# MPF Projects

We moved [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Fan-Tas-Tic Pinball]({% link _projects/fan_tas_tic.md %})
* [Earth Shaker Mod]({% link _projects/earth_shaker_mod.md %})
* [AF Tor Mod]({% link _projects/af_tor_mod.md %})
* [Tattoo Mystique]({% link _projects/tattoo_mystique.md %})
* [Zimball]({% link _projects/zimball.md %})

We know that there are a lot more projects. Let us know if you want to be listed here as well.

# 0.51 release

We released MPF 0.51.x and MPF-MC 0.51.4.

## Changes/New features

* No changes

## Bugfixes

* [Fix audio problems](https://github.com/missionpinball/mpf-mc/commit/7751cef626cae7fe0eeba2c4138f7ab6bb7d8982) - jab (0.51.4; based on [0.50 fix](https://github.com/missionpinball/mpf-mc/commit/e9d7f3aac92489ba8f987807aad5584938d77891#diff-b1084838e78cf0dc54bddd5026e1f747))

## Documentation

* No changes

# Dev release (future 0.52)

We pushed MPF 0.52.0-dev0 and MPF-MC 0.52.0-dev0.

## Changes/New features

* [OSC platform to control external lights](https://github.com/missionpinball/mpf/pull/1260) - jab based on [request in forum](https://groups.google.com/forum/#!topic/mpf-users/8JZbb_X__Rc)
* [Validate variables in variable_player](https://github.com/missionpinball/mpf/pull/1261) - jab based on [config in example](https://groups.google.com/forum/#!topic/mpf-users/v4b75FEQU70)
* [Placeholders for shots and shot_groups](https://github.com/missionpinball/mpf/pull/1262) - jab based on [question from mike wiz](https://groups.google.com/forum/#!topic/mpf-users/_EBF2tkfabI)
* [Better error messages for placeholders](https://github.com/missionpinball/mpf/commit/418b210e0e2bf847dcd66dbec5950d277828080c) - jab
* [Show proper error when fadecandy server is not running](https://github.com/missionpinball/mpf/pull/1263) - jab based on request from Brian Cox
* [Nicer output on startup errors](https://github.com/missionpinball/mpf/commit/55f449407d832e0bfa6f3403c19a3572ea621ee2) - jab
* [Show shutdown reason on exit of MPF](https://github.com/missionpinball/mpf/pull/1265) - jab
* [Show import error for pinproc](https://github.com/missionpinball/mpf/pull/1267) - jab
* [Add a segment display font](https://github.com/missionpinball/mpf-mc/commit/0dadad10eeaf01188e92016c90006ebb8b5b5933) - jab based on [example from BorgDog](https://groups.google.com/forum/#!topic/mpf-users/1wzjCo5pL0U)
* [Upstream Raspberry Pi DMD support](https://github.com/missionpinball/mpf/pull/1269) - jab based on [external platform from Michael Betz](https://github.com/yetifrisstlama/Fan-Tas-Tic-platform)

## Bugfixes

* [Fix audio problems](https://github.com/missionpinball/mpf-mc/commit/7751cef626cae7fe0eeba2c4138f7ab6bb7d8982) - jab (based on [0.50 fix](https://github.com/missionpinball/mpf-mc/commit/e9d7f3aac92489ba8f987807aad5584938d77891#diff-b1084838e78cf0dc54bddd5026e1f747))
* [Fix crash in achievments_group when setting auto_select and rotating an empty group](https://github.com/missionpinball/mpf/pull/1266/commits/4b366654b9975a7d00bad5ca028f863868ef47af) - jab
* [Only post select event of achievements on state change](https://github.com/missionpinball/mpf/pull/1266) - jab based on report from Brian Cox

## Documentation

* [How to change the size of switches and light in the MPF monitor](https://github.com/missionpinball/mpf-docs/commit/78bcd64254da3710423d5791ce6a067857c9c348) - jab based on questions from Jack Danger and Dan
* [Document StepStick stepper drivers in MPF](https://github.com/missionpinball/mpf-docs/commit/5f6b117f9e0cdae26514dc0e4d5846b83277a9e8) - jab based on [request from Tom](https://groups.google.com/forum/#!topic/mpf-users/ZgssCKBzvnA)
* [How to show virtual segment displays in MC](https://github.com/missionpinball/mpf-docs/commit/bda3bb1c11dbe3ea63c5d151299ab81f6c9ea7be) - jab based on [example from BorgDog](https://groups.google.com/forum/#!topic/mpf-users/1wzjCo5pL0U)
* [How to use multiple displays](https://github.com/missionpinball/mpf-docs/commit/a608639b21ff9cd62692fc12c7b05b8dc1ff5ee5) - jab based on [question in forum by Chris B and Snux](https://groups.google.com/forum/#!topic/mpf-users/2kjoLF_q9KA)
* [Credits mode tutorial](https://github.com/missionpinball/mpf-docs/commit/2df9021bd09fae9b6023ff9113c344ced45f5a22) - jab based on old tutorial
* [Tutorial on debugging memory leaks](https://github.com/missionpinball/mpf-docs/commit/e49caefff47f8b1af3642f946c1cc4d4c43f3a74) - jab based on question from Brian Cox
* [Document RPi DMD platform](https://github.com/missionpinball/mpf-docs/commit/d075be91f5592ead66469227186b0495b32d975d) - jab
* [How to subscribe variables in config players](https://github.com/missionpinball/mpf-docs/commit/b3c95c884cc2e622a6c017421216bb8ab4fa85c5) - jab based on [question](https://groups.google.com/forum/#!topic/mpf-users/nLnz5rM3Uus)

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Move libpinproc to a separate thread](https://github.com/missionpinball/mpf/pull/1195) - jab
* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen
* [Spike 2 support in mpf-spike-bridge](https://github.com/missionpinball/mpf-spike-bridge/pull/1) - jab and wolfmarsh

## Upcoming changes

* [Support for the Pololu Tic stepper controller](https://github.com/missionpinball/mpf/issues/1217) - wolfmarsh
* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab
* [Full support for LISY35](https://github.com/missionpinball/mpf/issues/1218) - jab

## Do you want to contribute?

A list of things where we would love contributions (not exclusive):

* Pictures for the following devices: [pop bumpers](http://docs.missionpinball.org/en/dev/mechs/pop_bumpers/index.html),
  [incandescant bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/matrix_lights.html),
  [GI bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [GI LEDs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [WS281x or serial LEDs](http://docs.missionpinball.org/en/dev/mechs/lights/leds.html),
  [data east optos](docs.missionpinball.org/en/dev/mechs/switches/optos.html),
  [dual wound coils](http://docs.missionpinball.org/en/dev/mechs/coils/dual_wound_coils.html),
  [coils](http://docs.missionpinball.org/en/dev/mechs/coils/index.html),
  [orbits](http://docs.missionpinball.org/en/dev/mechs/loops/index.html),
  [kickbacks](http://docs.missionpinball.org/en/dev/mechs/kickbacks/index.html),
  [kicking targets](http://docs.missionpinball.org/en/dev/mechs/targets/kicking_targets/index.html),
  [servos](http://docs.missionpinball.org/en/dev/mechs/servos/index.html),
  [accelerometer](http://docs.missionpinball.org/en/dev/mechs/accelerometers/index.html),
  [playfield](http://docs.missionpinball.org/en/dev/mechs/playfields/index.html),
  [flashers](http://docs.missionpinball.org/en/dev/mechs/lights/flashers.html),
  [flippers](http://docs.missionpinball.org/en/dev/mechs/flippers/index.html),
  [steppers](http://docs.missionpinball.org/en/dev/mechs/steppers/index.html),
  [score reels](http://docs.missionpinball.org/en/dev/mechs/score_reels/index.html),
  [diverters](http://docs.missionpinball.org/en/dev/mechs/diverters/index.html),
  [trough with optos](http://docs.missionpinball.org/en/dev/mechs/troughs/index.html) - please only send us picture where the rights belong to you
* [add an initial stepper device howto](http://docs.missionpinball.org/en/dev/mechs/steppers/index.html)
* Document asset pools such as [video_pools](http://docs.missionpinball.org/en/dev/config/video_pools.html), [image_pools](http://docs.missionpinball.org/en/dev/config/image_pools.html) or [show_pools](http://docs.missionpinball.org/en/dev/config/show_pools.html)
* [Create an electronical drawing for mechanical switches in matrix and on direct inputs](http://docs.missionpinball.org/en/dev/mechs/switches/mechanical_switches.html)
* [Document motors](http://docs.missionpinball.org/en/dev/mechs/motors/index.html)
* [Add an example or howto for timed switches](http://docs.missionpinball.org/en/dev/game_logic/timed_switches/index.html)
* [Add an example or howto for ball holds](http://docs.missionpinball.org/en/dev/game_logic/ball_holds/index.html)
* [Add an example or howto for combo switches](http://docs.missionpinball.org/en/dev/game_logic/combo_switches/index.html)
* [Add an example or howto for diverters](http://docs.missionpinball.org/en/dev/mechs/diverters/index.html)
* [Add an example or howto for shot_profiles](http://docs.missionpinball.org/en/dev/game_logic/shots/shot_profiles.html)
* [Adding more devices to the built-in service mode](https://github.com/missionpinball/mpf/issues/693)
* [More good first issues in MPF](https://github.com/missionpinball/mpf/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
* [More TODOs in the documentation](http://docs.missionpinball.org/en/dev/search.html?q=help_us_to_write_it&check_keywords=yes&area=default)

Other contributions are welcome as well.
Those are meant as starting point.
Let us know in the [forum](https://groups.google.com/forum/#!forum/mpf-users)
if you want to work on something or got questions.

## New contributors

Welcome  and .

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
