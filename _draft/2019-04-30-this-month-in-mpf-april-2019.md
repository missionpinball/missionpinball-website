---
layout: post
author: jab
title: This Month in MPF April 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in April 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* [The Awesome But Little Known Lightshow Creator For MPF]({% post_url 2019-04-07-the-awesome-but-little-known-lightshow-creator-for-mpf %}) 

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Apollo 11]({% link _projects/apollo_11.md %})
* [Judas Priest]({% link _projects/judas_priest.md %})
* [Pincraft]({% link _projects/pincraft.md %})
* [Metroid]({% link _projects/metroid.md %})
* [The Binding of Isaac]({% link _projects/binding_of_isaac.md %})
* [Legends of Camelot]({% link _projects/legends_of_camelot.md %})

We know that there are a lot more projects. Let us know if you want to be listed here as well (it does not matter in which stage your project is).

# 0.52 release

We released MPF 0.52.2 and MPF-MC 0.52.1.

## Changes

* No changes

## Bugfixes

* [Allow carousel mode during attract](https://github.com/missionpinball/mpf/pull/1326) - avanwinkle (backport; 0.52.2) 

# Dev release (future 0.53)

We pushed MPF 0.53.0-dev0 and MPF-MC 0.53.0-dev0.

## Changes/New features

* [Separate event handlers and code to catch incorrect arguments in custom code](https://github.com/missionpinball/mpf/pull/1327) - jab
* [Auto launch when machine is tilted](https://github.com/missionpinball/mpf/pull/1330) - jab based on [question from Philip D](https://groups.google.com/forum/#!topic/mpf-users/rjDghM-2XXk)
* [Show player and machine variables in the Text UI](https://github.com/missionpinball/mpf/pull/1328) - woosle1234
* [Allow dynamic values in timer control events](https://github.com/missionpinball/mpf/pull/1337) - avanwinkle based on report by wilder
* [Reduce default batch size for Spike LEDs](https://github.com/missionpinball/mpf/commit/e3ad5dded06c820db2ec38cbccdc3ed8f683480a) - jab based on tests by Dave
* [Custom events_when_added and events_when_removed for widgets](https://github.com/missionpinball/mpf-mc/pull/372) [[2]](https://github.com/missionpinball/mpf/pull/1338) - qcapen based on [feature request by cfbenn](https://github.com/missionpinball/mpf/issues/1332)
* [Better cache invalidation of config_spec cache](https://github.com/missionpinball/mpf/commit/d806ceecb0a53e61d3726471008611b229fb4fd7) - jab
* [Refactor Text UI to prevent text clutter](https://github.com/missionpinball/mpf/pull/1339) - jab
* [Allow user to disable ball search in a ball device](https://github.com/missionpinball/mpf/pull/1341) -  dziedada
* [Add control events to counters](https://github.com/missionpinball/mpf/pull/1342) - dziedada

## Bugfixes

* [Allow carousel mode during attract](https://github.com/missionpinball/mpf/pull/1325) - avanwinkle
* [Do not start highscore mode without a game](https://github.com/missionpinball/mpf/pull/1331) - jab based on report by wilder
* [Properly save window positions in MPF Monitor](https://github.com/missionpinball/mpf-monitor/commit/79bb049101b62bf846c4451ac462b0d0a4a7acaf) - jab based on [report by Greg](https://groups.google.com/forum/#!topic/mpf-users/JXB5Pv26Ces)

## Documentation

* [Document start_game_event and add_player_event](https://github.com/missionpinball/mpf-docs/commit/49b4bd34e1a8d675115c99bac1a05c9054921928) - jab
* [Add warnings about common ground to all coils](https://github.com/missionpinball/mpf-docs/commit/13efc1612aff5308239972383b7403bede0f8f3a) - jab 
* [More tags vs tokens in shows](https://github.com/missionpinball/mpf-docs/commit/3441c61471772745c299389481ff7d03945e5872) - jab
* [How to embed high score in attract mode](https://github.com/missionpinball/mpf-docs/commit/aa7fb941fbd39ab9d10c66735f4bb5de7493a94a) - jab based on [example by Greg](https://groups.google.com/forum/#!topic/mpf-users/TGp86erLGKc)
* [How to display a timer on a slide](https://github.com/missionpinball/mpf-docs/commit/5f9b640d36af055051adf15dba0ea2a0735f1dcd) - jab based on example from Coleman
* [Common pitfall with accruals](https://github.com/missionpinball/mpf-docs/pull/215) - colemanomartin
* [Enable of StepStick needs to be low not high](https://github.com/missionpinball/mpf-docs/pull/207) - colemanomartin
* [Add Multimorphic part numbers for breakout boards and LEDs](https://github.com/missionpinball/mpf-docs/commit/3482321d29872d1555399d345e2cc9e5c62f08c7) - jab
* [Document breakout boards for switches](https://github.com/missionpinball/mpf-docs/commit/7a6afed328a0ebfbe61bdafcd4cc5d7a9f51edef) - jab
* [More homebrew part numbers](https://github.com/missionpinball/mpf-docs/commit/49b398350341a8f781cbcf1e96647f8684c34cc8) - jab
* [Thermal considerations about resistors on Optos](https://github.com/missionpinball/mpf-docs/pull/216) - colemanomartin
* [Document rotation on widgets](https://github.com/missionpinball/mpf-docs/pull/218) - colemanomartin based on [question in forum](https://groups.google.com/forum/#!topic/mpf-users/v2uAIPbz8nA)
* [Update notes on rotation of widgets](https://github.com/missionpinball/mpf-docs/pull/217) - colemanomartin
* [Document custom widget events](https://github.com/missionpinball/mpf-docs/commit/497a4f53cf174bb2814680a1ded7875194ca9d0a) - qcapen 
* [How to configure tilt and change tilt slides](https://github.com/missionpinball/mpf-docs/commit/ec47267b2ace174480f7e90dc6875bafcc863203) - jab based on [example/question in the forum](https://groups.google.com/forum/#!topic/mpf-users/iHZxy9_eHPk)
* [Stern Spike Steppers](https://github.com/missionpinball/mpf-docs/commit/3aa75dc6c3bc47b5b56d32ee89f18b900b135e68) - jab

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

Welcome woosle1234 and dziedada.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
