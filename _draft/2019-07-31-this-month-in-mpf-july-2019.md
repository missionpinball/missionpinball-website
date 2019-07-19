---
layout: post
author: jab
title: This Month in MPF July 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in July 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* xx

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [xxx]({% link _projects/xxx.md %})


We know that there are a lot more projects. Let us know if you want to be listed here as well (it does not matter in which stage your project is).

# 0.52 release

We released MPF 0.52.3 and MPF-MC 0.52.4.

## Changes

* No changes

## Bugfixes

* 

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev42 and MPF-MC 0.53.0-dev5.

## Changes/New features

* [Segment display support for APC](https://github.com/missionpinball/mpf/pull/1388) - jab
* [Add token to slide_player to pass variables](https://github.com/missionpinball/mpf/pull/1389) and [MC](https://github.com/missionpinball/mpf-mc/pull/377) - jab based on [request in the forum by Greg](https://groups.google.com/forum/#!topic/mpf-users/ln2y_qxGRg4)
* [Increased light update throughput](https://github.com/missionpinball/mpf/pull/1390) - jab
* [Add express syntax for sound_player](https://github.com/missionpinball/mpf-mc/pull/378) - jab
* [Refactor machine variables](https://github.com/missionpinball/mpf/pull/1394) - pmansukhani
* [Tune shows and events](https://github.com/missionpinball/mpf/pull/1392) - jab
* [Setup improvements and wheels for OSX](https://github.com/missionpinball/mpf-mc/pull/379) - qcapen

## Bugfixes

* [Fix events_when_xxx on sounds](https://github.com/missionpinball/mpf-mc/pull/378) and [2](https://github.com/missionpinball/mpf/pull/1393) - qcapen and jab based on [report by Greg](https://groups.google.com/forum/#!topic/mpf-users/B8PF2WqFpYo)

## Documentation

* [Document wire-to-wire connectors](https://github.com/missionpinball/mpf-docs/pull/242) - ironspider
* [Add wiresheet for 7-segment displays with mypinballs controller](https://github.com/missionpinball/mpf-docs/pull/241) - unRARed
* [When Two Drop Targets Are Hit Simultaneously How Do I Keep Two Sounds From Playing](https://github.com/missionpinball/mpf-docs/commit/7909751f5f0b09727e0c68e8b561d76b3e4e4ef3) - qcapen
* [Typos](https://github.com/missionpinball/mpf-docs/pull/243), [2](https://github.com/missionpinball/mpf-docs/pull/244), [3](https://github.com/missionpinball/mpf-docs/pull/245) - ironspider

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

Welcome unRARed and pmansukhani.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
