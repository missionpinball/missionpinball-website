---
layout: post
author: jab
title: This Month in MPF November 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in November 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Brooks and Dunn]({% link _projects/brooks_and_dunn.md %})
* [Cthulhu - Attack on Arkham]({% link _projects/cthulhu_attack_on_arkham.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anthing wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.52 release

We released MPF 0.52.7 and MPF-MC 0.52.5.

## Bugfixes

* No changes

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev77 and MPF-MC 0.53.0-dev14.

## Changes/New features

* [Generic high score mode which works for DMD and LCD](https://github.com/missionpinball/mpf/pull/1447), [2](https://github.com/missionpinball/mpf-mc/commit/efb6bfe5e58826e6545998a0ae9d7108e51ca1e3) - jab
* [Improve correctness, speed and error messages of config validation](https://github.com/missionpinball/mpf/pull/1455) - jab
* [Option to ignore checksum errors in Spike](https://github.com/missionpinball/mpf/pull/1456) - jab
* [Support new input command for Spike FW 0.49+](https://github.com/missionpinball/mpf/pull/1457) - jab
* [Implement over current detection for Spike](https://github.com/missionpinball/mpf/commit/f8da2cf9b063a342f9ca15c7d84090f853a3465c) - jab
* [Arbitrary start state for state_machines](https://github.com/missionpinball/mpf/pull/1458) - avanwinkle
* [Configurable debounce times and FW 0.49+ for Spike](https://github.com/missionpinball/mpf/pull/1460) - jab
* [Coil priorities in hw rules for Spike FW 0.49+](https://github.com/missionpinball/mpf/pull/1462) - densminger and jab
* [Placeholders in ball save active_time](https://github.com/missionpinball/mpf/pull/1463) - avanwinkle
* [Autodetect FAST ports](https://github.com/missionpinball/mpf/pull/1464) - avanwinkle
* [Improve robustness of LISY protocol](https://github.com/missionpinball/mpf/pull/1466) - jab

## Bugfixes

* [Fix setting number of LEDs per node in Spike FW 0.49+](https://github.com/missionpinball/mpf/pull/1461) - densminger and jab

## Documentation

* [Documentation (integration) tests with MC to make sure examples always work](https://github.com/missionpinball/mpf-docs/pull/269) - jab
* [Integration test for shots and widgets](https://github.com/missionpinball/mpf-docs/commit/9e952c2d55c7b20880fe7016b9ed9756b39b0519) - jab
* [Remove Python 3.4 references from docs](https://github.com/missionpinball/mpf-docs/pull/268) - cfbenn
* [Upgrade instructions for old to new kivy version](https://github.com/missionpinball/mpf-docs/commit/14736abf223f252d41b9bdaf65826afbbf92740d) - jab
* [Document numlock keyboard issue](https://github.com/missionpinball/mpf-docs/pull/271) - mwiz
* [Document common problems with OPP on Ubuntu](https://github.com/missionpinball/mpf-docs/commit/2e0bdf0fcb4641a6d3fc08fb2503dec2da0e29f5) - jab
* [Extend APC documentation](https://github.com/missionpinball/mpf-docs/commit/f70701129cdee00a36e65e07afd875205ce9bb11) - jab
* [Document how to install MPF Spike bridge with FW 0.49+](https://github.com/missionpinball/mpf-docs/pull/270) - densminger

## IDE support

* [Emacs instructions](https://github.com/missionpinball/mpf-ls/pull/6) - seanirby
* [Support goto definition and hover + mode support](https://github.com/missionpinball/mpf-ls/pull/7) - jab
* [Basic diagnostics](https://github.com/missionpinball/mpf-ls/pull/8) - jab

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
