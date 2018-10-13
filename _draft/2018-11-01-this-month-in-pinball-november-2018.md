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

* 

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

We know that there are a lot more projects. Let us know if you want to be listed here as well.

# Current stable release (0.50)

We released MPF 0.50.16 and MPF-MC 0.50.8 with bugfixes and backports.

## Changes

No changes

## Bugfixes

* 

## Documentation

No changes

# Dev release (future 0.51)

We pushed MPF 0.51.0-dev-11 and MPF-MC 0.51.0-dev.2.

## Changes/New features

* [Support multiple (stacked) style values for widgets](https://github.com/missionpinball/mpf-mc/pull/349) - avanwinkle
* [Validate that ball_count for multiballs is the right range](https://github.com/missionpinball/mpf/pull/1229) - jab based on [question from Alex](https://groups.google.com/forum/#!topic/mpf-users/jQTwpofBysA)
* [Better error when showing images too early](https://github.com/missionpinball/mpf-mc/pull/350) - jab based on [question from Brian C](https://groups.google.com/forum/#!topic/mpf-users/iMivocg70BQ)
* [Allow variable_players outside game modes for machine variables](https://github.com/missionpinball/mpf/pull/1231) - jab
* [Allow widget styles to set z values](https://github.com/missionpinball/mpf-mc/pull/351) - avanwinkle
* [Only reset drop target banks if a target is down](https://github.com/missionpinball/mpf/pull/1236) - jab based on [request from Mark M](https://groups.google.com/forum/#!topic/mpf-users/kHq3dM1PMyo)
* [Add support for flipper tapping for OPP](https://github.com/missionpinball/mpf/pull/1238) - jab and Hugh based on [forums discussion](https://groups.google.com/forum/#!topic/mpf-users/pKfmv_lmuDc)

## Bugfixes

* [Fix iMC initialisation](https://github.com/missionpinball/mpf-mc/pull/352) - avanwinkle

## Documentation

* [Document how to use machine and player variables from code](https://github.com/missionpinball/mpf/pull/1232) - jab
* [Document multiple styles for widgets](https://github.com/missionpinball/mpf-docs/pull/180) - avanwinkle
* [Document how to use start button for mode selection without added new players](https://github.com/missionpinball/mpf-docs/commit/946426c043a34af7cccd48027fa06fa658799019) - jab based on [example provided by alex](https://groups.google.com/forum/#!topic/mpf-users/e3emzNIxZp0)
* [Document which hardware rules are used in MPF](https://github.com/missionpinball/mpf-docs/commit/d9d95dd66795e2301731eacbc7e1bb7932374f99) - jab based on [discussion in the forum](https://groups.google.com/forum/#!topic/mpf-users/pKfmv_lmuDc)

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Reusing named widgets](https://github.com/missionpinball/mpf-mc/pull/353) - avanwinkle

## Upcoming changes/Not landed yet

* [Support for the Pololu Tic stepper controller](https://github.com/missionpinball/mpf/issues/1217) - wolfmarsh
* Stern Spike 2 support - wolfmarsh and jab
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
  [coils](http://docs.missionpinball.org/en/dev/mechs/coils/index.html)
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
  [diverters](http://docs.missionpinball.org/en/dev/mechs/diverters/index.html)
  [trough with optos](http://docs.missionpinball.org/en/dev/mechs/troughs/index.html) - please only send us picture where the rights belong to you
* [Document the stepper device config options](http://docs.missionpinball.org/en/dev/config/steppers.html) and [add an initial stepper device howto](http://docs.missionpinball.org/en/dev/mechs/steppers/index.html)
* Document asset pools such as [video_pools](http://docs.missionpinball.org/en/dev/config/video_pools.html), [image_pools](http://docs.missionpinball.org/en/dev/config/image_pools.html) or [show_pools](http://docs.missionpinball.org/en/dev/config/show_pools.html)
* [Create an electronical drawing for mechanical switches in matrix and on direct inputs](http://docs.missionpinball.org/en/dev/mechs/switches/mechanical_switches.html)
* [Add an example or howto for timed switches](http://docs.missionpinball.org/en/dev/game_logic/timed_switches/index.html)
* [Add an example or howto for ball holds](http://docs.missionpinball.org/en/dev/game_logic/ball_holds/index.html)
* [Add an example or howto for combo switches](http://docs.missionpinball.org/en/dev/game_logic/combo_switches/index.html)

Other contributions are welcome as well.
Those are meant as starting point.
Let us know in the [forum](https://groups.google.com/forum/#!forum/mpf-users) if you want to work on anything or got questions.

## New contributors

Welcome x

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
