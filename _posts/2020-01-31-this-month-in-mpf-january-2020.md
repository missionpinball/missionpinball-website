---
layout: post
author: jab
title: This Month in MPF January 2020
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in January 2020?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Sonic the Hedgehog Spinball]({% link _projects/sonic_the_hedgehog_spinball.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anthing wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.53 release

We released MPF 0.53.2 and MPF-MC 0.53.0.

## Bugfixes

* [Fix crash in some MC players](https://github.com/missionpinball/mpf/commit/71bd5af7ca2fca80918a5b6ed8213b98f4cc5f2e) - jab (backport)
* [Fix fast shutdown bug when an error occured](https://github.com/missionpinball/mpf/commit/15b8b6a8928400c82f7f73488f617504c51a55cc) - jab (backport)

# Dev release (future 0.54)

We pushed MPF 0.54.4-dev2 and MPF-MC 0.54.0-dev0.

## Changes/New features

* [Deduplicate asyncio code](https://github.com/missionpinball/mpf/pull/1488) - jab
* [Support more Pin2DMD hardware options](https://github.com/missionpinball/mpf/pull/1491) - jab
* [Do not flush in pypinproc](https://github.com/missionpinball/pypinproc/commit/b631d57265e35ea32618677cae79c8ad1e0d1ffc) - jab
* [Do not call flush on write_data in pypinproc to speed up LEDs on PD-LED](https://github.com/missionpinball/libpinproc/commit/5bb2146d3e655515c08e41d184f2a6bcce4667d4) - jab

## Bugfixes

* [Fix fast shutdown bug when an error occured](https://github.com/missionpinball/mpf/commit/26f434888fa6a283ff1cbb98a6432bbb2844e7de) - jab
* [Prevent crashes from empty platform configs](https://github.com/missionpinball/mpf/commit/37a4f433f3dc659db505104abda6644453d5a279) - jab
* [Fix crash in some MC players](https://github.com/missionpinball/mpf/commit/377fab44fe9b158a208f6f508b60dbddebcad621) - jab

## Documentation

* [Release notes to 0.53](https://github.com/missionpinball/mpf-docs/commit/b415e0b6abe3a7201b79cf07fca71a8e0dfa5d42) - jab
* [Extend fadecandy documentation](https://github.com/missionpinball/mpf-docs/commit/9d6f5fa1c5a523f6c34acbafc20f43d9cf05bddd) - jab
* [Document Pin2DMD](https://github.com/missionpinball/mpf-docs/commit/4aa03a2f74e414034658cc750bd82b91884bc5cf) - jab
* [Faster docs generation](https://github.com/missionpinball/mpf-docs/commit/7ea6b86420275967efbde1ad73f13c717fbf7fc7) - jab
* [Remove stuff from roadmap which has been implemented](https://github.com/missionpinball/mpf-docs/commit/ef4a5ad2cd7cc0a8043a4c78cb44ff67373c4326) - jab
* [Link to our libpinproc fork](https://github.com/missionpinball/mpf-docs/commit/066e3bdf6925569059f2315b5db0e10242c2da93) - jab
* [Add link to VS Redistributables for pypinproc on Windows](https://github.com/missionpinball/mpf-docs/commit/7f28db099f01d2b0d6451a0f4f7ef028a3299d65) - jab
* [Fix DMD font style names](https://github.com/missionpinball/mpf-docs/pull/273) - kevwilde


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

Welcome kevwilde.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
