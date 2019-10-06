---
layout: post
author: jab
title: This Month in MPF September 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in September 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [1985 Tag Team]({% link _projects/1985_tag_team.md %})
* [Dead Flip Pin]({% link _projects/dead_flip.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anthing wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.52 release

We released MPF 0.52.7 and MPF-MC 0.52.5.

## Bugfixes

* [Fix polarity issue with P-Roc and WPC](https://github.com/missionpinball/mpf/commit/cc3e74bd2515d3625a62bcd7e97f4028192b1e0c) - jab (backport 0.52.5)
* [Fix crash with uvloop](https://github.com/missionpinball/mpf/commit/b36cd2019554b8f8ac7b591738ca0501ca355c4c) - jab (backport 0.52.6)
* [Fix diverter activation on startup](https://github.com/missionpinball/mpf/commit/9b0649cc5f9cdce41c752ae19c7c52cbce9857e8) - jab (original fix by GabeKnuth; backport 0.52.7)
* [Prevent high score mode start before game](https://github.com/missionpinball/mpf/commit/fd6d02cbc1f9da3954f2d81702af2852db1204d5) - jab (backport 0.52.7)

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev62 and MPF-MC 0.53.0-dev12.

## Changes/New features

* [Support daisy chaining in the Pololu Maestro](https://github.com/missionpinball/mpf/pull/1410) - jab
* [Expose P-Roc hardware version as machine variable](https://github.com/missionpinball/mpf/commit/7be95d1cc79dfee12d44ff25b0972444121ff6bc) - jab
* [Placeholders for shoot_again in multiball](https://github.com/missionpinball/mpf/pull/1404) - pmansukhani
* [Support show_tokens with placeholders in shot_profiles](https://github.com/missionpinball/mpf/pull/1414) - jab
* [Regression Test for Diverters (for a bug which was fixed during refactoring)](https://github.com/missionpinball/mpf/commit/4a9251b819e470b2072dbf634e26d1b4c1e5daec) - jab
* [Expose MPF and MC version in MPF-MC on connect](https://github.com/missionpinball/mpf-mc/commit/732cf02e5aefedbba4e9af72d7c0c7f1aa8b93a5) - jab
* [Support pulse power in P/P3-Roc](https://github.com/missionpinball/mpf/pull/1418) - jab
* [Add Scaffolding CLI to MPF](https://github.com/missionpinball/mpf/pull/1419) - jab
* [Optimized Service Mode for LCDs](https://github.com/missionpinball/mpf/commit/6e09beca89f18f718402f3780cd42fb624b3d948) - jab

 
## Bugfixes

* [Fix inverted condition on show player conditions](https://github.com/missionpinball/mpf/pull/1407) - avanwinkle
* [Prevent false positive duplicate numbers in virtual platform](https://github.com/missionpinball/mpf/pull/1409) - jab
* [Prevent crash in Text UI](https://github.com/missionpinball/mpf/commit/b121d1e91245e99a88ef68463a67dfcb9f8a154a) - jab

 
## Documentation

* [Add LISY35 to WPC section](https://github.com/missionpinball/mpf-docs/commit/865bd788752b4f2f56c9695d4d49c6901ae37e69) - jab
* [Document machine variables](https://github.com/missionpinball/mpf/commit/a433f72cee16101f37b66f81dcb5c944888a7571) and [more](https://github.com/missionpinball/mpf-docs/commit/dcb0364e4cfa409567c3e3315f432d774e9cbf4a) - jab
* [Add images for coils, buttons, flasher, up-down-ramps and diverters](https://github.com/missionpinball/mpf-docs/pull/261) -  kevinleedrum
* [Improve skill shot documentation](https://github.com/missionpinball/mpf-docs/commit/6a93a3d8b08028418911ad485b50f07cffc4952a) - jab
* [Improve service mode documentation](https://github.com/missionpinball/mpf-docs/commit/ce3373e970bb5c7461ebceb1375bb804041c2031) - jab 

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
  [orbits](http://docs.missionpinball.org/en/dev/mechs/loops/index.html),
  [kickbacks](http://docs.missionpinball.org/en/dev/mechs/kickbacks/index.html),
  [kicking targets](http://docs.missionpinball.org/en/dev/mechs/targets/kicking_targets/index.html),
  [accelerometer](http://docs.missionpinball.org/en/dev/mechs/accelerometers/index.html),
  [playfield](http://docs.missionpinball.org/en/dev/mechs/playfields/index.html),
  [flippers](http://docs.missionpinball.org/en/dev/mechs/flippers/index.html),
  [score reels](http://docs.missionpinball.org/en/dev/mechs/score_reels/index.html),
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

Welcome kevinleedrum.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
