---
layout: post
author: jab
title: This Month in MPF March 2020
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in March 2020?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anything wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.53 release

We released MPF 0.53.2 and MPF-MC 0.53.3.

## Bugfixes

* [Disable Mac Wheels as they caused install issues](https://github.com/missionpinball/mpf-mc/commit/d7563436ea54cc5b491c7d098b518ee9d5f1ebd6) - jab (backport; 0.52.3)

# Dev release (future 0.54)

We pushed MPF 0.54.0-dev.18 and MPF-MC 0.54.0-dev.5.

## Changes/New features

* [Turn off incands at start for OPP](https://github.com/missionpinball/mpf/commit/e0e711d1a7c525474aa12e09a98a86bd043895cc) - jab
* [Remove space separated lists](https://github.com/missionpinball/mpf/pull/1505) - jab
* [Support delayed pulses in autofires and kickbacks and implement it for OPP](https://github.com/missionpinball/mpf/pull/1507) - jab
* [Refactor config loading](https://github.com/missionpinball/mpf/pull/1506) - jab
* [Support serial LEDs in OPP on new boards](https://github.com/missionpinball/mpf/pull/1508) - jab
* [Enable dot priority syntax everywhere](https://github.com/missionpinball/mpf/commit/9fda4065f8084781c47f65c61a47ba0d9fd8ddef) - jab
* [Remove dash syntax for control events](https://github.com/missionpinball/mpf/commit/27833c715a22f2a9f430b5d18db7161a1b2895f4) - jab
* [Unity config spec loading for mpf and mc](https://github.com/missionpinball/mpf/commit/c9802a7f65da2e7184c67eefad3f3a05b0f1cc5a) - jab
* [Remove ball locks as they have been replaced by multiball_locks and ball_holds](https://github.com/missionpinball/mpf/commit/ab45e683e9b434cde420b001236051587cec7fe3) - jab
* [Dynamic value for keep_multiplier in bonus mode](https://github.com/missionpinball/mpf/pull/1510) - seanirby
* [Batch commands for PD-LED](https://github.com/missionpinball/mpf/commit/9b08f849ad88e1f6d810a54235dc2da5696961a0) - jab
* [Inputs on Neopixel wings in OPP](https://github.com/missionpinball/mpf/commit/65615b2d36b0741d6f029e47ea28e89bdd208446) - jab
* [Add mpf build production_bundle](https://github.com/missionpinball/mpf/commit/2a91b5f436c9e3c745eb6127f056b40e5f3aad1e) - jab
* [Log config load times](https://github.com/missionpinball/mpf/commit/81e9750f4ea0c0b2c5fb42ee4cb59cdf7d97f84e) - jab
* [Interface for binary data storage (instead of yaml) for high scores and audits](https://github.com/missionpinball/mpf/commit/32221dcb6b108fb8f655950aa8c88a8f6fa26769) - jab
* [Test software update in service mode](https://github.com/missionpinball/mpf-mc/commit/cce63720ef5c09140b427cff156721f459deb260) - jab
* [Fix asset loading in overloaded modes](https://github.com/missionpinball/mpf-mc/commit/d0095cb6825a783cecbe91513ea0c7e22879ece8) - jab
* [Remove space separated lists in MC](https://github.com/missionpinball/mpf-mc/pull/396) - jab
* [Refactor Config Loading in MC](https://github.com/missionpinball/mpf-mc/pull/398) - jab
* [Build MC on Python 3.5 to 3.7](https://github.com/missionpinball/mpf-mc/commit/1843582c154bc5db0a7ada04a0c0508d8013b519) - jab
* [Support Production Config Bundles in MC](https://github.com/missionpinball/mpf-mc/commit/f55b7ee8a7247654858b5d90e0f33896730bae58) - jab

## Bugfixes

* [Fix asset loading when overloading a mode](https://github.com/missionpinball/mpf/commit/56fc2580a1356f1640cb8ea321bcb6c7224d19b1) fixes [bug 1366](https://github.com/missionpinball/mpf/issues/1366) - jab
* [Detect missing curly backets in conditional events](https://github.com/missionpinball/mpf/commit/82fc767ae10079dad062be75f30a91661254a3ee) fix [bug 1497](https://github.com/missionpinball/mpf/issues/1497) - jab
* [Prevent adding player during high score of a one ball game](https://github.com/missionpinball/mpf/pull/1509) - seanirby
* [Fix config spec for hardware section](https://github.com/missionpinball/mpf/commit/03349317fb331129bf8a12a0830938475ebd86f6) - jab
* [Fix servos on PD-LED with new libpinproc](https://github.com/missionpinball/mpf/commit/f417215b90236b3f0f3970e4d00a41e80a595b75) and [add a test](https://github.com/missionpinball/mpf/commit/1fe2ef21cb28731ba35cb16817be54fd962ab70d) - jab
* [Fix subscriptions in logic blocks](https://github.com/missionpinball/mpf/commit/794a8b875bd486dba8aa380377de9795fea4088e) - jab
* [Fix broken subscriptions during player change](https://github.com/missionpinball/mpf/commit/9b795c9db594f4ef7426e75023fcde110547fc76) - jab
* [Disable Mac Wheels as they caused install issues](https://github.com/missionpinball/mpf-mc/commit/921323f0ec0c149b1e670077e9a11607502f38f1) - jab

## Documentation

* [Dual-coil diverters](https://github.com/missionpinball/mpf-docs/commit/faba0261923d6aadf2fbaa5aca8d07c1556dd769) - jab
* [Add generic part numbers](https://github.com/missionpinball/mpf-docs/commit/c0a8eabd0df380c7e3cd0bd12883c64bf72e389e) - jab
* [Document Motors](https://github.com/missionpinball/mpf-docs/commit/eaf74ead18f712c403d4223bbf46ab8110713375) - jab
* [Document Shakers](https://github.com/missionpinball/mpf-docs/commit/3cbe8dc9192f2f042133a0123b779c3fa87d34c6) - jab
* [Add Pop Bumper Images](https://github.com/missionpinball/mpf-docs/commit/12cd1357114906631d696a5cf15688ad3a5e47bf) - aaronmatthies
* [Add example how to end a game by long-pressing start](https://github.com/missionpinball/mpf-docs/commit/ce58da4473499bf9ec3134ef3cd67b72e7fd95c4) - jab
* [Describe PSU magic](https://github.com/missionpinball/mpf-docs/commit/5db12ab87ea6dc8191db137ae76cbfcd6e10898b) - jab
* [How to fix drop target reset issues](https://github.com/missionpinball/mpf-docs/commit/f8786db15c04701679d1dbe432c2a6868ac34770) - jab
* [Document Pololu Tic](https://github.com/missionpinball/mpf-docs/commit/277814e78bc4deddb73edf35bd2617e926c0849e) - jab
* [Reference placeholders in bonus mode](https://github.com/missionpinball/mpf-docs/pull/286) - seanirby
* [Keyboard tutorial](https://github.com/missionpinball/mpf-docs/commit/9ac2ef49331529d4846aeaa284bf957e3d3a65c0) - jab
* [Integrating Logic Blocks and Lights](https://github.com/missionpinball/mpf-docs/commit/ab322dd528e459ac4d9ca94920c1e0e7cab2e8e1) - jab
* [Tutorial on Counter and Slide integration](https://github.com/missionpinball/mpf-docs/commit/5ac152d2d1c82e9306808890b018f6434b8f7604) - jab
* Update all config references: [OPP](https://github.com/missionpinball/mpf-docs/commit/01bbf59eaffbb8ca69b01b18b1b75e2d79e30cbc), [Pin2DMD and P-Roc](https://github.com/missionpinball/mpf-docs/commit/707c36c24623f64a60bce2b73d15c854577c066a) and many more - jab
* [How to drain all balls and keep the ball live](https://github.com/missionpinball/mpf-docs/pull/288/files), [2](https://github.com/missionpinball/mpf-docs/pull/287) -  mwiz
* [Improve achievments documentation](https://github.com/missionpinball/mpf-docs/pull/289) - atummons


Have a look at the [dev documentation](https://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen

## Upcoming changes

* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab

## Do you want to contribute?

A list of things where we would love contributions (not exclusive):

* Pictures for the following devices:
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

Welcome atummons!

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
