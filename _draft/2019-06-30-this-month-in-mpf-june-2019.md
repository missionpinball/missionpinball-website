---
layout: post
author: jab
title: This Month in MPF June 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in June 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* 


# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [xxx!]({% link _projects/xxx.md %})

We know that there are a lot more projects. Let us know if you want to be listed here as well (it does not matter in which stage your project is).

# 0.52 release

We released MPF 0.52.2 and MPF-MC 0.52.1.

## Changes

* No changes

## Bugfixes

* No changes

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev34 and MPF-MC 0.53.0-dev4.

## Changes/New features

* [Add links to the docs to warnings and errors](https://github.com/missionpinball/mpf/pull/1380) - jab
* [Improve fake game in tests to handle multiball drains](https://github.com/missionpinball/mpf/commit/458927fca909510ef5df643e6947a886862a2aa9) - jab
* [Remove Windows Python 3.4 build of MPF-MC](https://github.com/missionpinball/mpf-mc/commit/ad6e0fdb5bcd4bdad142b1ac563696f61b60733d) - qcapen
* [Improve sound_loop_player design](https://github.com/missionpinball/mpf-mc/pull/374) - qcapen
* [Python 3.7 support for Windows in MPF-MC](https://github.com/missionpinball/mpf-mc/commit/4dda4261fe527fec829e9e3e3488af8e407a7daf) - qcapen
 
## Bugfixes

* [Fix regression in multiball counting](https://github.com/missionpinball/mpf/pull/1377) - avanwinkle
* [Fix sound_loop_player bugs](https://github.com/missionpinball/mpf-mc/commit/f14b5214246188e3cd61d9eef2193f17ff9548e5) - qcapen
* [Fix Mac build](https://github.com/missionpinball/mpf-mc/commit/2bd209465b6b599f2ae937892e909cf1470fd5fd) - qcapen

## Documentation

* [Log mesage reference section](https://github.com/missionpinball/mpf-docs/commit/30258abce59ea1d810827fdcc178938073394f26) - jab
* [Add score slide to tutorial step 17](https://github.com/missionpinball/mpf-docs/pull/237) - Coleman
* [Fix instructions on how to install a specific MPF version](https://github.com/missionpinball/mpf-docs/pull/238) [2](https://github.com/missionpinball/mpf-docs/pull/239) - mfulleratlassian

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

Welcome mfulleratlassian and .

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
