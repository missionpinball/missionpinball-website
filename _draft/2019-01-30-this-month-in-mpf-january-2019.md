---
layout: post
author: jab
title: This Month in MPF January 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in January 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* [Python 3.7 support in MPF 0.52]({% post_url 2019-01-25-python-3.7-support %}) - jab

# MPF Projects

We moved [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [The Black Hole]({% link _projects/black_hole.md %})
* [Aziz Pinball]({% link _projects/aziz.md %})
* [The Fight Club]({% link _projects/fight_club.md %})


We know that there are a lot more projects. Let us know if you want to be listed here as well.

# 0.51 release

We released MPF 0.51.x and MPF-MC 0.51.x.

## Changes/New features

* No changes

## Bugfixes

* 

## Documentation

* No changes

# Dev release (future 0.52)

We pushed MPF 0.52.0-dev0 and MPF-MC 0.52.0-dev0.

## Changes/New features

* [Improve USB latency for I2C in pypinproc](https://github.com/missionpinball/pypinproc/pull/5) - jab based on suggestion by rosh
* [Only enable AC relay by default during the game. Keep it off in attract](https://github.com/missionpinball/mpf/pull/1289) - snux
* [Ball Routing device to route balls to certain devices](https://github.com/missionpinball/mpf/pull/1291) - jab
* [Support for the Pololu Tic stepper controller](https://github.com/missionpinball/mpf/pull/1293) - wolfmarsh
* [Update Smartmatrix Teensy Code Example for New Cookie](https://github.com/missionpinball/mpf/pull/1295) - aaronmatthies and eli
* [Placeholders in event_player based on event parameters](https://github.com/missionpinball/mpf/pull/1297) - avanwinkle
* [Update ruamel yaml parser](https://github.com/missionpinball/mpf/pull/1298) - jab
* [Use newer cython to support Python 3.7](https://github.com/missionpinball/mpf-debian-installer/commit/532d8757c078ef568b6a9d3473a1db63d35e84ef) - jab
* [Add Python 3.7 support to MPF](https://github.com/missionpinball/mpf/pull/1300) - jab

## Bugfixes

* [Properly support external platforms in MC](https://github.com/missionpinball/mpf-mc/pull/361) - jab based on [report by TheLegoMoviePinball](https://groups.google.com/forum/#!topic/mpf-users/okl8PjXrlWI) 
* [Honour -a and -A option when loading config_spec in MPF](https://github.com/missionpinball/mpf/pull/1280) and [MC](https://github.com/missionpinball/mpf-mc/pull/362) - jab based on [report by TheLegoMoviePinball](https://groups.google.com/forum/#!topic/mpf-users/okl8PjXrlWI)
* [Honour slide parameter in inactive slides](https://github.com/missionpinball/mpf-mc/pull/363) - avanwinkle
* [Fix crash in coil_player when using off action](https://github.com/missionpinball/mpf/pull/new/coil_player_crash) - jab based on [bug reported by snux](https://github.com/missionpinball/mpf/issues/1282)
* [Fix iMC startup crash](https://github.com/missionpinball/mpf-mc/pull/364) - jab based on [report by snux](https://groups.google.com/forum/#!topic/mpf-users/YLrh6RKlx0s)
* [Fix sound_queue for on demand sounds](https://github.com/missionpinball/mpf/pull/1299) - avanwinkle

## Documentation

* Monitorable properties for [shots](https://github.com/missionpinball/mpf/pull/1287) and [shot_groups](https://github.com/missionpinball/mpf-docs/commit/f2b1833153fb391d6316ed8afb18761eaa580854) - jab based on [question by snux](https://groups.google.com/forum/#!topic/mpf-users/cVnmhJIN1tM)  
* [Document recycle settings for more platforms](https://github.com/missionpinball/mpf-docs/commit/cec753171700165814d0853684e6ac9c6357df76) - jab based on [question by Cole M](https://groups.google.com/forum/#!topic/mpf-users/qGVVwTbYnrA)
* [Explain logic and modes in MPF](https://github.com/missionpinball/mpf-docs/pull/197) - colemanomartin
* [Notes on case-sensitivity](https://github.com/missionpinball/mpf-docs/pull/195) - colemanomartin
* [Explain A and C side preference in System11/Snux](https://github.com/missionpinball/mpf-docs/pull/194) - snux
* [Fix typos](https://github.com/missionpinball/mpf-docs/pull/196) - travisbmartin
* [Document monitorable properties and event in logic blocks](https://github.com/missionpinball/mpf-docs/commit/7a03143a5ebf571f6092ebf4b28a7b7282420584) - jab
* [Example for conditionals in log](https://github.com/missionpinball/mpf-docs/commit/34e8403e29d3292d82ff768bac95c400f16191c4) - jab
* [Update Smartmatrix documentation for new cookie](https://github.com/missionpinball/mpf-docs/pull/198) - aaronmatthies
* [Document start/launcher/tournament buttons](https://github.com/missionpinball/mpf-docs/commit/1073eb379d827037f094123d73d4180ab433d8e3) - jab
* Document part numbers and voltages for [bulbs, flashers](https://github.com/missionpinball/mpf-docs/commit/59c62c471e8c9237b33bfa424f192eb332d8d500), [GIs and popbumpers](https://github.com/missionpinball/mpf-docs/commit/ddfa77cfbfd6fa37ecf2b36f911d4220f84a9d8f) and [LEDs](https://github.com/missionpinball/mpf-docs/commit/24bbc32b25a75580d9407a12676d12cd14af9136) - jab 
* [Up-Down ramps](https://github.com/missionpinball/mpf-docs/commit/79166be8691b92e2c8f3a77c0f76ce299ad56759) - jab

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen
* [Spike 2 support in mpf-spike-bridge](https://github.com/missionpinball/mpf-spike-bridge/pull/1) - jab and wolfmarsh

## Upcoming changes

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

Welcome aaronmatthies and eli.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
