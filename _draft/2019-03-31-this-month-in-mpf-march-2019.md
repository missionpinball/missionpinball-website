---
layout: post
author: jab
title: This Month in MPF March 2019
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in March 2019?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

*

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [xx]({% link _projects/xx.md %})

We know that there are a lot more projects. Let us know if you want to be listed here as well.

# 0.52 release

We released MPF 0.52.1 and MPF-MC 0.52.1.

## Changes/New features

* No changes

## Bugfixes

* [Fix crash after config error](https://github.com/missionpinball/mpf/commit/c3a3f1f9d7b620e531c2adf78773556883be3624) - jab based on report by Wilder (backport)

## Documentation

* No changes


# Dev release (future 0.53)

We pushed MPF 0.53.0-dev8 and MPF-MC 0.53.0-dev2.

## Changes/New features

* [Spike-MPF bridge in Rust](https://github.com/missionpinball/mpf-spike/commit/529ac6d7d047ef8d74ce2e4555a910a4ddf190c5) - jab
* [Use new Spike-MPF bridge in MPF](https://github.com/missionpinball/mpf/commit/089f7e48008ab0e82d3d8712ef812ea636975933) - jab
* [Use a better default for max_servo_value on PD-LEDs](https://github.com/missionpinball/mpf/commit/9fbbd9bbe1367566e5defda0a2914f75db1635d2) - jab
* [Allow reverse sorted highscore categories](https://github.com/missionpinball/mpf/pull/1296) - yensho
* [Light batching in Spike for better light sync](https://github.com/missionpinball/mpf/pull/1313) - jab based on [request by Dave](https://groups.google.com/forum/#!topic/mpf-users/WHRLH0lGZL0)
* [Read ticks_per_second per node for Spike](https://groups.google.com/forum/#!topic/mpf-users/WHRLH0lGZL0) - jab 
* [Reliable speed/flow control in Spike](https://github.com/missionpinball/mpf/pull/1314) - jab
* [Initial Spike 2 support for the mpf-spike bridge](https://github.com/missionpinball/mpf-spike/commit/e234336f504c40a5050220e00b5baa049d659819) - jab
* [Limit light batch size in Spike to prevent bus desync](https://github.com/missionpinball/mpf/commit/f64d46689235bb1e4d5abaa63de6d5cf39a4c661) - jab
* [Ignore duplicate handler warnings during init](https://github.com/missionpinball/mpf/pull/1316) - avanwinkle
* [Add support for steppers in Spike](https://github.com/missionpinball/mpf/pull/1317) - jab
* [Support Spike 2 backlight](https://github.com/missionpinball/mpf/commit/3bd30788613c687674d4e3c8bbace77691e0d1f5) - jab
* [Support Spike 1 and Spike 2 backlight in bridge](https://github.com/missionpinball/mpf-spike/commit/9ee733992c127050cb31fe79d8ab0f8d89871467) - jab
* [Servo and Steppers as Diverters](https://github.com/missionpinball/mpf/pull/1321) - jab

## Bugfixes

* [Fix crash in debug message for duplicate priorities](https://github.com/missionpinball/mpf/commit/7a3dad3ef3366b33f4fa77e45abfa54026faa76c) - jab based on report from Dave
* [Fix crash after config error](https://github.com/missionpinball/mpf/commit/4613cfe3b0c3d8199eaaf633f3626c228714faab) - jab based on report by Wilder
* [Properly use priority in widget_player when the slide is not active and becomes active later](https://github.com/missionpinball/mpf-mc/pull/371) - avanwinkle

## Documentation

* [Document new Spike bridge](https://github.com/missionpinball/mpf-docs/commit/6be23912212478beaa35356226ef86d37cd2cf49) - jab
* [Document steppers and add images](https://github.com/missionpinball/mpf-docs/pull/208) - colemanomartin
* [Image an image of a servo](https://github.com/missionpinball/mpf-docs/commit/4da3b0a4ca6a0910d2ed89065d61411f92a91f90) - colemanomartin
* [Better stepper example code](https://github.com/missionpinball/mpf-docs/pull/211) - colemanomartin
* [Details about PD-LED servo fine tuning](https://github.com/missionpinball/mpf-docs/pull/210) - colemanomartin
* [Clarify monitorable servo properties](https://github.com/missionpinball/mpf-docs/pull/209) - colemanomartin
* [Document showcreator](https://github.com/missionpinball/mpf-docs/commit/29f7312c4efff3ace0ed4d77f9ec255e18aa166f) - jab
* [Fix typo](https://github.com/missionpinball/mpf-docs/pull/212) - cfbenn
* [Docs for named_colors and example for dynamic widgets](https://github.com/missionpinball/mpf-docs/pull/213) - avanwinkle based on [request by Philip](https://groups.google.com/forum/#!topic/mpf-users/_WCjW4_9Hic)
* [Better examples for sequence_shots](https://github.com/missionpinball/mpf-docs/pull/214) - colemanomartin
* [More text for the showcreator](https://github.com/missionpinball/mpf-docs/commit/7a3aeb1c30ea19474b9815e55ada5e287572086f) - jab
* [Light_player examples](https://github.com/missionpinball/mpf-docs/commit/639dbe2276e9404d4307d497ff7a065795050dbe) - jab
* [How to use shows in shows](https://github.com/missionpinball/mpf-docs/commit/70b2d0498a1c121e8d0f7b4f0fe2885630505ab0) - jab
* [Windows install error and fix](https://github.com/missionpinball/mpf-docs/commit/2d855b79ba24ef8492e20020d7f6dac861a50b34) - jab based on error from Jordan
* [Document common logic block questions](https://github.com/missionpinball/mpf-docs/commit/03f60656b795a775e538ea97a693960e4bcaae0b) - jab based on [question in forum from iizi](https://groups.google.com/forum/#!topic/mpf-users/X5HYU60gjoc)
* [Document servos and steppers as diverters](https://github.com/missionpinball/mpf-docs/commit/17651d0902b1a09d6d9ff91b890b851518cc2ad3) - jab based on [question in forum](https://groups.google.com/forum/#!topic/mpf-users/YZlYmkEzAkw)

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
  [accelerometer](http://docs.missionpinball.org/en/dev/mechs/accelerometers/index.html),
  [playfield](http://docs.missionpinball.org/en/dev/mechs/playfields/index.html),
  [flashers](http://docs.missionpinball.org/en/dev/mechs/lights/flashers.html),
  [flippers](http://docs.missionpinball.org/en/dev/mechs/flippers/index.html),
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

Welcome yensho and yyy.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
