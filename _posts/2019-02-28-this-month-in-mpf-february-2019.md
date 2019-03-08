---
layout: post
author: jab
title: This Month in MPF February 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in February 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* [MPF 0.52 has been released]({% post_url 2019-02-02-mpf-0-52-released %})
* [Segment Displays on light drivers]({% post_url 2019-02-10-segment-displays-on-light-drivers %}) - jab

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Celts]({% link _projects/celts.md %})

We know that there are a lot more projects. Let us know if you want to be listed here as well.

# 0.52 release

We released MPF 0.52.1 and MPF-MC 0.52.1.

## Changes/New features

* No changes

## Bugfixes

* [Fix some yaml parsing errors](https://github.com/missionpinball/mpf/pull/1303) - jab
* [Fix error with Python 3.7](https://github.com/missionpinball/mpf-mc/pull/370) - avanwinkle 
* [Fix driver stuck on in rules in P/P3-Roc](https://github.com/missionpinball/mpf/pull/1308) - jab [0.52.1; backport]

## Documentation

* [Extend Multimorphic PowerEntry board documentation](https://github.com/missionpinball/mpf-docs/pull/203) - colemanomartin
* [Fix tutorial step 18](https://github.com/missionpinball/mpf-docs/commit/fe6afd6878f66b18d7e49e972f1444ab9363e9eb) - jab based on [question by Pablo](https://groups.google.com/forum/#!topic/mpf-users/czoLprd5pL8)


# Dev release (future 0.53)

We pushed MPF 0.53.0-dev0 and MPF-MC 0.53.0-dev0.

## Changes/New features

* [Support segment displays connected to normal light of a platform](https://github.com/missionpinball/mpf/pull/1305) - jab
* [Batch LED updates for PD-LED and P/P3-Roc to prevent bus overflows](https://github.com/missionpinball/mpf/pull/1310) - jab
* [Make separate thread configurable in P/P3-Roc and reduce IPC overhead](https://github.com/missionpinball/mpf/pull/1311) - jab
* [Highlight settings in service mode](https://github.com/missionpinball/mpf/pull/1309) - avanwinkle

## Bugfixes

* [Fix some yaml parsing errors](https://github.com/missionpinball/mpf/pull/1303) - jab
* [Fix error with Python 3.7](https://github.com/missionpinball/mpf-mc/pull/370) - avanwinkle
* [Fix driver stuck on in rules in P/P3-Roc](https://github.com/missionpinball/mpf/pull/1308) - jab 
* [Do not crash in service cli when playing invalid shows](https://github.com/missionpinball/mpf/pull/1312) - jab

## Documentation

* [Extend Multimorphic PowerEntry board documentation](https://github.com/missionpinball/mpf-docs/pull/203) - colemanomartin
* [Center Post Ball Save Example](https://github.com/missionpinball/mpf-docs/commit/aaef1046b6d3f4443fa21e61decb333aa91d4605) - mwiz
* [Part numbers for trough opto boards](https://github.com/missionpinball/mpf-docs/commit/f4f66e49a6946a9e24ae1636d3f7d6a5faa961bc) - jab
* [Image for Center Post](https://github.com/missionpinball/mpf-docs/commit/908995a8e7a0e941dd461dfbc1c1bfbabc5d0f81) - swizzlefish 
* [Improve game mode example](https://github.com/missionpinball/mpf-docs/pull/204) - gregsealby
* [Fix typos](https://github.com/missionpinball/mpf-docs/pull/205), [fix2](https://github.com/missionpinball/mpf-docs/pull/206) - densminger
* [Extend documentation for multiple screens](https://github.com/missionpinball/mpf-docs/commit/793d1652c308bb7dfce2daaa5f7774db9071394b) - jab based on [question by Haggis and solution by Snux](https://groups.google.com/forum/#!topic/mpf-users/vs62guaHNE4)
* [Fix tutorial step 18](https://github.com/missionpinball/mpf-docs/commit/05aa704487a1117a14c3ff201809081f5a67a9fa) - jab based on [question by Pablo](https://groups.google.com/forum/#!topic/mpf-users/czoLprd5pL8)

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen
* [Spike 2 support in mpf-spike-bridge](https://github.com/missionpinball/mpf-spike-bridge/pull/1) - jab and wolfmarsh
* [New Spike bridge with less switch latency in Rust](https://github.com/missionpinball/mpf-spike) - jab

## Upcoming changes

* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab
* [Full support for LISY35](https://github.com/missionpinball/mpf/issues/1218) - jab and bontango

## Do you want to contribute?

A list of things where we would love contributions (not exclusive):

* Pictures for the following devices: [pop bumpers](http://docs.missionpinball.org/en/dev/mechs/pop_bumpers/index.html),
  [incandescant bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/matrix_lights.html),
  [GI bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [GI LEDs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
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

Welcome gregsealby and densminger.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
