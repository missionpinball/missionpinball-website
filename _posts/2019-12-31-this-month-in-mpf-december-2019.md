---
layout: post
author: jab
title: This Month in MPF December 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in December 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Quidditch]({% link _projects/quidditch.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anthing wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.52 release

We released MPF 0.52.10 and MPF-MC 0.52.5.

## Bugfixes

* [Fix duplicate BCP messages which could trigger duplicate sounds or widgets](https://github.com/missionpinball/mpf/pull/1486) - jab (backport)
* [Also advance score reels for non-active players](https://github.com/missionpinball/mpf/pull/1472) - jab (backport)
* [Fix score reel crash](https://github.com/missionpinball/mpf/commit/a7263d8d42df01b6978cbc155fe668bc21f4d6e3) - jab (backport)

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev83 and MPF-MC 0.53.0-dev16.

## Changes/New features

* [Improve placeholder performance by evaluating them only when needed](https://github.com/missionpinball/mpf/pull/1469) - jab
* [Update ruamel.yaml to improve the install experience on Windows](https://github.com/missionpinball/mpf/pull/1476) - jab
* [Benchmark and tune/cache placeholder parsing](https://github.com/missionpinball/mpf/pull/1478) - jab
* [Priorities in ball_holds and ball_locks](https://github.com/missionpinball/mpf/pull/1479) - avanwinkle
* [Batch light for PD-LED](https://github.com/missionpinball/mpf/pull/1481) - jab
* [Benchmark and tune event performance](https://github.com/missionpinball/mpf/pull/1483) - jab
* [Extend combo_switches to include the triggering switch in the event](https://github.com/missionpinball/mpf/pull/1480) - avanwinkle
* [Initial Pin2DMD support (not yet working)](https://github.com/missionpinball/mpf/pull/1484) - jab
* [Option to ignore FAST RGB CPU crashes](https://github.com/missionpinball/mpf/pull/1482) - avanwinkle
* [Tracing for libpinproc calls](https://github.com/missionpinball/mpf/commit/9c7f3af27d4bdb91a67d80f6f0b43550d4607a3b) - jab
* [Software update via Service mode](https://github.com/missionpinball/mpf/pull/1487) - jab
* [Add tests for accrual restarts](https://github.com/missionpinball/mpf/pull/1470) - jab

## Bugfixes

* [High score mode should run before match mode](https://github.com/missionpinball/mpf/pull/1467) - jab
* [Prevent crash in text ui on unknown switch event](https://github.com/missionpinball/mpf/pull/1468) - jab
* [Also advance score reels for non-active players](https://github.com/missionpinball/mpf/pull/1471) - jab
* [Consider OPP firmware version per chain instead of globally](https://github.com/missionpinball/mpf/pull/1474) - jab
* [Fix sequence_shots with a single switch and delay](https://github.com/missionpinball/mpf/pull/1473) - jab
* [Fix crash in score reels](https://github.com/missionpinball/mpf/pull/1475) - jab
* [Prevent crash in variable player when adding a variable for a non-exising player](https://github.com/missionpinball/mpf/pull/1477) - jab
* [Prevent duplicate BCP messages which could trigger duplicate sounds or widgets](https://github.com/missionpinball/mpf/pull/1485) - jab

## Documentation

* [Improve OPP docs](https://github.com/missionpinball/mpf-docs/commit/2e0bdf0fcb4641a6d3fc08fb2503dec2da0e29f5) - jab
* [APC documentation](https://github.com/missionpinball/mpf-docs/commit/f70701129cdee00a36e65e07afd875205ce9bb11) - jab
* [Document how to use newer Spike 1 firmwares with MPF](https://github.com/missionpinball/mpf-docs/pull/270) - densminger
* [Typo](https://github.com/missionpinball/mpf-docs/commit/8a16696104fad7d1de030ea04788bbc62f8c8ee9) - jab
* [Show config tests in docs](https://github.com/missionpinball/mpf-docs/commit/4bb13cbf915ff687a780b6477c453c95035b2c8a) - jab
* [Example for other player scoring](https://github.com/missionpinball/mpf-docs/commit/987de22b1fa4db47bf3a1b2c273983ae4b3311af) - jab


Have a look at the [dev documentation](https://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen

## Upcoming changes

* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab

## Do you want to contribute?

A list of things where we would love contributions (not exclusive):

* Pictures for the following devices: [pop bumpers](https://docs.missionpinball.org/en/dev/mechs/pop_bumpers/index.html),
  [incandescant bulbs](https://docs.missionpinball.org/en/dev/mechs/lights/matrix_lights.html),
  [GI bulbs](https://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [GI LEDs](https://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [data east optos](https://docs.missionpinball.org/en/dev/mechs/switches/optos.html),
  [dual wound coils](https://docs.missionpinball.org/en/dev/mechs/coils/dual_wound_coils.html),
  [orbits](https://docs.missionpinball.org/en/dev/mechs/loops/index.html),
  [kickbacks](https://docs.missionpinball.org/en/dev/mechs/kickbacks/index.html),
  [kicking targets](https://docs.missionpinball.org/en/dev/mechs/targets/kicking_targets/index.html),
  [accelerometer](https://docs.missionpinball.org/en/dev/mechs/accelerometers/index.html),
  [playfield](https://docs.missionpinball.org/en/dev/mechs/playfields/index.html),
  [score reels](https://docs.missionpinball.org/en/dev/mechs/score_reels/index.html),
  [trough with optos](https://docs.missionpinball.org/en/dev/mechs/troughs/index.html) - please only send us picture where the rights belong to you
* Document asset pools such as [video_pools](https://docs.missionpinball.org/en/dev/config/video_pools.html), [image_pools](https://docs.missionpinball.org/en/dev/config/image_pools.html) or [show_pools](https://docs.missionpinball.org/en/dev/config/show_pools.html)
* [Create an electronical drawing for mechanical switches in matrix and on direct inputs](https://docs.missionpinball.org/en/dev/mechs/switches/mechanical_switches.html)
* [Document motors](https://docs.missionpinball.org/en/dev/mechs/motors/index.html)
* [Add an example or howto for timed switches](https://docs.missionpinball.org/en/dev/game_logic/timed_switches/index.html)
* [Add an example or howto for ball holds](https://docs.missionpinball.org/en/dev/game_logic/ball_holds/index.html)
* [Add an example or howto for combo switches](https://docs.missionpinball.org/en/dev/game_logic/combo_switches/index.html)
* [Add an example or howto for diverters](https://docs.missionpinball.org/en/dev/mechs/diverters/index.html)
* [Adding more devices to the built-in service mode](https://github.com/missionpinball/mpf/issues/693)
* [Good first issues in MPF](https://github.com/missionpinball/mpf/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
* [Good first issues in MPF-MC](https://github.com/missionpinball/mpf-mc/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
* [Good first issues in MPF-Monitor](https://github.com/missionpinball/mpf-monitor/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
* [More TODOs in the documentation](https://docs.missionpinball.org/en/dev/search.html?q="Help+us+to+write+it"&check_keywords=yes&area=default)

Other contributions are welcome as well.
Those are meant as starting point.
Let us know in the [forum](https://groups.google.com/forum/#!forum/mpf-users)
if you want to work on something or got questions.

## New contributors

Welcome seanirby.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
