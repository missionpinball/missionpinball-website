---
layout: post
author: jab
title: This Month in MPF October 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in October 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Proto1]({% link _projects/proto1.md %})
* [Rollr Girlz]({% link _projects/rollr_girlz.md %})
* [Steam Punk Royale]({% link _projects/steampunk_royale.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anthing wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.52 release

We released MPF 0.52.7 and MPF-MC 0.52.5.

## Bugfixes

* No changes in October

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev64 and MPF-MC 0.53.0-dev14.

## Changes/New features

* [Suggestions on config typos](https://github.com/missionpinball/mpf/pull/1424) - jab 
* [Copy light positions in scaffolding CLI from monitor to MPF for display_light_player](https://github.com/missionpinball/mpf/pull/1423) - jab
* [Add start_enabled to achievements and refactor code](https://github.com/missionpinball/mpf/pull/1426) - jab
* [Add unselect_events to achievements and more cleanup](https://github.com/missionpinball/mpf/pull/1429) - jab
* [More achievement refactoring](https://github.com/missionpinball/mpf/pull/1431) - jab
* [Refactored test cases](https://github.com/missionpinball/mpf/pull/1432) - jab
* [Drop Python 3.4 support](https://github.com/missionpinball/mpf/pull/1433) - jab
* [Turn device collections into native dicts](https://github.com/missionpinball/mpf/pull/1435) - jab
* [Led_color default show now supports all default show_tokens](https://github.com/missionpinball/mpf/pull/1441) - jab
* [Log asset loading times for tuning](https://github.com/missionpinball/mpf/pull/1442) - jab
* [Show shot state in MPF-monitor](https://github.com/missionpinball/mpf/pull/1446) - jab
* [Validate transitions in state_machines](https://github.com/missionpinball/mpf/pull/1445) - jab
* [Improve config parsing/validation](https://github.com/missionpinball/mpf/pull/1452) - jab
* [Nicer errors and suggestions in shows](https://github.com/missionpinball/mpf/pull/1453) - jab
* [Improve install and dependency manangement for Max and Linux](https://github.com/missionpinball/mpf-mc/pull/387) - jab
* [Improve build and install on Windows](https://github.com/missionpinball/mpf-mc/pull/388) - jab
* [Lazy loading for zipped image sequences to speed up game startup](https://github.com/missionpinball/mpf-mc/pull/389) - jab

## Bugfixes

* [Scaffolding from any path (just like other commands)](https://github.com/missionpinball/mpf/pull/1421) - jab
* [Set default enable/disable_event for magnets](https://github.com/missionpinball/mpf/pull/1422) - jab
* [Bring back state_names_to_not_rotate in shot_profiles](https://github.com/missionpinball/mpf/pull/1430) - jab to fix [bug reported by Greg](https://groups.google.com/forum/#!searchin/mpf-users/state_names_to_not_rotate%7Csort:date/mpf-users/kpFWgW2QgBM/3_Q0CIIfDAAJ)
* [Prevent false positive duplicate events handlers](https://github.com/missionpinball/mpf/pull/1436) - jab based on [report from Greg](https://groups.google.com/forum/#!topic/mpf-users/bLnPsXiBrTI)
* [Fix crash in show player](https://github.com/missionpinball/mpf/pull/1440) - jab
* [Fix config validation](https://github.com/missionpinball/mpf/pull/1448) - kevinleedrum
* [Fix reenabling of achievement_groups](https://github.com/missionpinball/mpf/pull/1443) - jab
* [Improve error urls](https://github.com/missionpinball/mpf/pull/1444) - jab
* [Fix call to libpinproc for pulse_power](https://github.com/missionpinball/mpf/commit/f32606bf8722fe501190be4ff3619924970821c1) - jab
* [Do not crash on headless display_light_player](https://github.com/missionpinball/mpf-mc/commit/04c1963bbdc17e63d92598de1b5caf37506059fc) - jab

 
## Documentation

* [Document text_ui section](https://github.com/missionpinball/mpf-docs/pull/260) - avanwinkle
* [Fix typos](https://github.com/missionpinball/mpf-docs/pull/264) and [grammar](https://github.com/missionpinball/mpf-docs/pull/266) - catrinaisahuman
* [Fix typo in path](https://github.com/missionpinball/mpf-docs/pull/265) - arthurlutz
* [Added flipper image](https://github.com/missionpinball/mpf-docs/pull/267) - tpilewicz

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen

## Upcoming changes

* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab

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

Welcome catrinaisahuman, tpilewicz and arthurlutz.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
