---
layout: post
author: jab
title: This Month in Pinball November 2018
tags: [this_month_in_pinball, MPF]
---
What happened in MPF-land in November 2018?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News


# MPF Projects

Some active publicly documented projects by MPF users.

* [The Crazy Mansion](https://pinside.com/pinball/forum/topic/the-crazy-mansion-by-the-pinball-amigos)
* [The Nightmare Before Christmas](https://pinside.com/pinball/forum/topic/the-nightmare-before-christmas)
* [Minions Pinball](https://pinside.com/pinball/forum/topic/we-are-building-a-minions-pinball-updates-every-friday)
* [The Last Starfighter](https://pinside.com/pinball/forum/topic/southern-california-homebrew-anyone-interested/)
* [Good vs Evil Head2Head](https://pinside.com/pinball/forum/topic/head2head-custom-pinball-machine-good-vs-evil)
* [Spaceballs - The Pin](https://pinside.com/pinball/forum/topic/spaceballs-the-pin/)
* [Queen Pinball](https://pinside.com/pinball/forum/topic/flash-retheme-project/)
* [HotRod](https://pinside.com/pinball/forum/topic/gottlieb-hot-rod-a-tribute-to-classic-em-pinball)
* [Gravity Falls](https://pinside.com/pinball/forum/topic/gravity-falls)
* [Haggis Pinball](https://www.youtube.com/watch?v=Qezv5beKBqM)
* [Powerman 5000](https://github.com/travisbmartin/powerman)
* [Doctor Who Redux](https://github.com/travisbmartin/doctorwho)

We know that there are a lot more projects. Let us know if you want to be listed here as well.

# Current stable release (0.50)

We released MPF 0.50.20 and MPF-MC 0.50.8 with bugfixes and backports.

## Changes

* 

## Bugfixes

* 

## Documentation

No changes

# Dev release (future 0.51)

We pushed MPF 0.51.0-dev-11 and MPF-MC 0.51.0-dev.2.

## Changes/New features

* 
## Bugfixes

* 

## Documentation

* 

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Move libpinproc to a separate thread](https://github.com/missionpinball/mpf/pull/1195) - jab
* [Reusing named widgets](https://github.com/missionpinball/mpf-mc/pull/353) - avanwinkle
* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen
* [Spike 2 support in mpf-spike-bridge](https://github.com/missionpinball/mpf-spike-bridge/pull/1) - jab and wolfmarsh

## Upcoming changes

* [Support for the Pololu Tic stepper controller](https://github.com/missionpinball/mpf/issues/1217) - wolfmarsh
* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab
* More stepper and servo hardware - jab
* [Full support for LISY35](https://github.com/missionpinball/mpf/issues/1218) - jab

## Do you want to contribute?

A list of things where we would love contributions (not exclusive):

* [Adding more devices to the built-in service mode](https://github.com/missionpinball/mpf/issues/693)
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
  [drop target banks](http://docs.missionpinball.org/en/dev/mechs/targets/drop_targets/drop_target_bank.html)
  [servos](http://docs.missionpinball.org/en/dev/mechs/servos/index.html),
  [accelerometer](http://docs.missionpinball.org/en/dev/mechs/accelerometers/index.html),
  [playfield](http://docs.missionpinball.org/en/dev/mechs/playfields/index.html),
  [flashers](http://docs.missionpinball.org/en/dev/mechs/lights/flashers.html),
  [flippers](http://docs.missionpinball.org/en/dev/mechs/flippers/index.html),
  [score reels](http://docs.missionpinball.org/en/dev/mechs/score_reels/index.html),
  [diverters](http://docs.missionpinball.org/en/dev/mechs/diverters/index.html),
  [trough with optos](http://docs.missionpinball.org/en/dev/mechs/troughs/index.html) - please only send us picture where the rights belong to you
* [Document the stepper device config options](http://docs.missionpinball.org/en/dev/config/steppers.html) and [add an initial stepper device howto](http://docs.missionpinball.org/en/dev/mechs/steppers/index.html)
* Document asset pools such as [video_pools](http://docs.missionpinball.org/en/dev/config/video_pools.html), [image_pools](http://docs.missionpinball.org/en/dev/config/image_pools.html) or [show_pools](http://docs.missionpinball.org/en/dev/config/show_pools.html)
* [Create an electronical drawing for mechanical switches in matrix and on direct inputs](http://docs.missionpinball.org/en/dev/mechs/switches/mechanical_switches.html)
* [Document motors](http://docs.missionpinball.org/en/dev/mechs/motors/index.html)
* [Add an example or howto for timed switches](http://docs.missionpinball.org/en/dev/game_logic/timed_switches/index.html)
* [Add an example or howto for ball holds](http://docs.missionpinball.org/en/dev/game_logic/ball_holds/index.html)
* [Add an example or howto for combo switches](http://docs.missionpinball.org/en/dev/game_logic/combo_switches/index.html)
* [Add an example or howto for diverters](http://docs.missionpinball.org/en/dev/mechs/diverters/index.html)
* [Add an example or howto for shot_profiles](http://docs.missionpinball.org/en/dev/game_logic/shots/shot_profiles.html)
* [More good first issues in MPF](https://github.com/missionpinball/mpf/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
* [More TODOs in the documentation](http://docs.missionpinball.org/en/dev/search.html?q=help_us_to_write_it&check_keywords=yes&area=default)

Other contributions are welcome as well.
Those are meant as starting point.
Let us know in the [forum](https://groups.google.com/forum/#!forum/mpf-users)
if you want to work on something or got questions.

## New contributors

Welcome xxx

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
