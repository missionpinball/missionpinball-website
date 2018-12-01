---
layout: post
author: jab
title: This Month in Pinball November 2018
tags: [this_month_in_pinball, MPF]
---
What happened in MPF-land in November 2018?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* [We released MPF 0.51]({% post_url 2018-11-24-mpf-0-51-released %})
* [Crazy Mansion, Minions Pinball and Good vs Evil at the Dutch Pinball Open](https://www.pinballnews.com/site/2018/11/18/dpo-expo-2018/)
* There seems to be a [sound issue in 0.51](https://groups.google.com/forum/#!topic/mpf-users/K6Q8l1K9ORE). We are working on that.

# MPF Projects

Some active publicly documented projects by MPF users.

* [The Crazy Mansion](https://pinside.com/pinball/forum/topic/the-crazy-mansion-by-the-pinball-amigos)
* [The Nightmare Before Christmas](https://pinside.com/pinball/forum/topic/the-nightmare-before-christmas)
* [Minions Pinball](https://pinside.com/pinball/forum/topic/we-are-building-a-minions-pinball-updates-every-friday)
* [The Last Starfighter](https://pinside.com/pinball/forum/topic/southern-california-homebrew-anyone-interested/)
* [Good vs Evil Head2Head](https://pinside.com/pinball/forum/topic/head2head-custom-pinball-machine-good-vs-evil)
* [Spaceballs - The Pin](https://pinside.com/pinball/forum/topic/spaceballs-the-pin/)
* [Queen Pinball](https://pinside.com/pinball/forum/topic/flash-retheme-project/)
* [HotRod](https://pinside.com/pinball/forum/topic/gottlieb-hot-rod-a-tribute-to-classic-em-pinball)
* [Gravity Falls](https://pinside.com/pinball/forum/topic/gravity-falls)
* [Haggis Pinball](https://www.youtube.com/watch?v=Qezv5beKBqM)
* [Powerman 5000](https://github.com/travisbmartin/powerman)
* [Doctor Who Redux](https://github.com/travisbmartin/doctorwho)
* [Forbidden Planet](https://pinside.com/pinball/forum/topic/john-treadeaus-forbidden-planet/) (new)
* [The Lego Movie](https://thelegomoviepinball.wordpress.com/) (french) (new)
* [Custom Raspberry](https://github.com/vgrillot/mpf) and [Arduino MPF platform](https://github.com/vgrillot/arduinball) (new)
* [DIY Pinball CAN Platform](http://diypinball.ca/) (new)
* [Fan-Tas-Tic Platform](https://github.com/yetifrisstlama/Fan-Tas-Tic-Firmware) (new)

We know that there are a lot more projects. Let us know if you want to be listed here as well.

# Old stable release (0.50)

We released MPF 0.50.21 and MPF-MC 0.50.8 with bugfixes and backports.
It will be maintained for a while with bugfixes.
However, upgrading should be fairly easy for most people so don't expect
maintainance for more than a few more month.
Let us know if you got troubles upgrading.

## Changes

* No changes

## Bugfixes

* [Prevent lags in LISY](https://github.com/missionpinball/mpf/pull/1249) - jab (backport; 0.50.21)

## Documentation

* No changes

# 0.51 release

We released MPF 0.51.1 and MPF-MC 0.51.3.

## Changes/New features

* [Add new mode_will_start hook for custom code](https://github.com/missionpinball/mpf/pull/1247) - Lamoraldus based on [discussion in forum](https://groups.google.com/forum/#!topic/mpf-users/D0W3pacTGUg)
* [Reusing named widgets](https://github.com/missionpinball/mpf-mc/pull/353) - avanwinkle
* [Support external platforms via entry_points](https://github.com/missionpinball/mpf/pull/1248) - jab
* [Refresh Smartmatrix DMDs periodically](https://github.com/missionpinball/mpf/pull/1250) - jab
* [Support Servos on PD-LED](https://github.com/missionpinball/mpf/pull/1253) - jab with help from gstellenberg ([announcement](https://www.multimorphic.com/news/servo-and-stepper-motor-control-in-pd-led-v3/))
* [Support Steppers on PD-LED/New stepper device interface](https://github.com/missionpinball/mpf/pull/1255) - jab with help from gstellenberg
* [Experimental external Philips Hue platform](https://github.com/missionpinball/mpf-hue-platform) - jab based on [code from  Philip D](https://groups.google.com/forum/#!topic/mpf-users/e5dv9j71BUE)
* [Support config specs for external platforms via entry_points](https://github.com/missionpinball/mpf/pull/1252) - jab

## Bugfixes

* [Prevent lags in LISY](https://github.com/missionpinball/mpf/pull/1249) - jab
* [Reallow playfield_active on switches in shots](https://github.com/missionpinball/mpf/commit/9c4940fb92c9c87a1d6d9aaf49531e4861ec3ce1) - jab based on feedback from Philip D. (backport)
* [Pin to old kivy dependencies because Windows bugs](https://github.com/missionpinball/mpf-mc/commit/a8330136cd799b5ec5b92184f7f24922547f511e) - jab based on feedback by multiple users (backport; see: [Kivy bug](https://github.com/kivy/kivy/issues/5916))

## Documentation

* [Fix typos and links](https://github.com/missionpinball/mpf-docs/pull/187) - zach27
* [Notes on using multiple playfields](https://github.com/missionpinball/mpf-docs/commit/ddcc16252cc783a4aab42c5f372085349914e10f) - jab based on [discussion in forum](https://groups.google.com/forum/#!topic/mpf-users/tnmvTI9J_O8)
* [Animating a progress bar](https://github.com/missionpinball/mpf-docs/commit/b272f836598d13562f41f99007f27f13278a0f9d) - based on [discussion in forum](https://groups.google.com/forum/#!topic/mpf-users/n2Shn9wDfUc)
* [Adding a picture of a drop target bank](https://github.com/missionpinball/mpf-docs/commit/38e8e8bba4ffaead3c6c0e5a1f88300c570aa312) - coleman
* [Fix typos](https://github.com/missionpinball/mpf-docs/pull/188) - travisbmartin
* [Update stepper documentation](https://github.com/missionpinball/mpf-docs/commit/6f588482e0fe51a112052a16c1cd2a587d35e7c5) - jab
* [Document PD-LED steppers, servos and serial LEDs](https://github.com/missionpinball/mpf-docs/commit/324a5cfc77061a6756f99d8a62b0ad1148aa843c) - jab

# Dev release (future 0.52)

We pushed MPF 0.52.0-dev0 and MPF-MC 0.52.0-dev0.

## Changes/New features

* [Refactor lights on a driver into separate platform](https://github.com/missionpinball/mpf/pull/1258) - jab
* [Support StepStick/DRV8825 on digital outputs](https://github.com/missionpinball/mpf/pull/1259) - jab based on [request from Tom](https://groups.google.com/forum/#!topic/mpf-users/ZgssCKBzvnA)

## Bugfixes

* [Reallow playfield_active on switches in shots](https://github.com/missionpinball/mpf/commit/9c4940fb92c9c87a1d6d9aaf49531e4861ec3ce1) - jab based on feedback from Philip D. 
* [Pin to old kivy dependencies because Windows bugs](https://github.com/missionpinball/mpf-mc/commit/a8330136cd799b5ec5b92184f7f24922547f511e) - jab based on feedback by multiple users (see: [Kivy bug](https://github.com/kivy/kivy/issues/5916))

## Documentation

* [Better playlist example](https://github.com/missionpinball/mpf-docs/commit/43249a87a52376230e8665ab777819ae696e4c7e) - jab based on [example from Brian C](https://groups.google.com/forum/#!topic/mpf-users/gxr5oTbmDrk) 

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Move libpinproc to a separate thread](https://github.com/missionpinball/mpf/pull/1195) - jab
* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen
* [Spike 2 support in mpf-spike-bridge](https://github.com/missionpinball/mpf-spike-bridge/pull/1) - jab and wolfmarsh
* [OSC platform to control external lights](https://github.com/missionpinball/mpf/pull/1260) - jab based on [request in forum](https://groups.google.com/forum/#!topic/mpf-users/8JZbb_X__Rc)

## Upcoming changes

* [Support for the Pololu Tic stepper controller](https://github.com/missionpinball/mpf/issues/1217) - wolfmarsh
* [Stern Spike 2 support](https://github.com/missionpinball/mpf/issues/1246) - wolfmarsh and jab
* [Full support for LISY35](https://github.com/missionpinball/mpf/issues/1218) - jab

## Do you want to contribute?

A list of things where we would love contributions (not exclusive):

* Pictures for the following devices: [pop bumpers](http://docs.missionpinball.org/en/dev/mechs/pop_bumpers/index.html),
  [incandescant bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/matrix_lights.html),
  [GI bulbs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [GI LEDs](http://docs.missionpinball.org/en/dev/mechs/lights/gis.html),
  [WS281x or serial LEDs](http://docs.missionpinball.org/en/dev/mechs/lights/leds.html),
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

Welcome Lamoraldus and zach27.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
