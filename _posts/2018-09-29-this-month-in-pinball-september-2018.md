---
layout: post
author: jab
title: This Month in Pinball September 2018
tags: [this_month_in_pinball, MPF]
---
What happened in MPF-land in September 2018?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# News

* [HotRod and OPP.. what happened?](https://openpinballproject.wordpress.com/2018/06/27/6-26-2018-hot-rod-and-opp-what-happened/) - Hugh from OPP
* [HotRod and OPP and MPF]({% post_url 2018-09-23-hothot-and-opp-and-mpf %}) - jab (as response to Hugh)
* [LISY35 for Bally/Stern machine between 1977 and 1985](https://pinside.com/pinball/forum/topic/lisy35-help-with-bally-lamp-driver-code-needed) - MPF will support this platform soon
* [MPF Stickers](https://groups.google.com/forum/#!topic/mpf-users/_Hfof-FKqcs)

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

We know that there are a lot more projects. Let us know if you want to be listed here as well.

# Current stable release (0.50)

We released MPF 0.50.16 and MPF-MC 0.50.8 with bugfixes and backports.

## Changes

No changes

## Bugfixes

* [Fix mode events when starting/stopping mode from BCP](https://github.com/missionpinball/mpf/issues/1215) - jab based on report by Travis Martin (backport)
* [Fix display_light_player crash when used in mode](https://github.com/missionpinball/mpf/pull/1224) - jab (backport)
* [Fix crash in BCP with MPF Monitor](https://github.com/missionpinball/mpf/pull/1226) - jab based on [report from alex](https://groups.google.com/forum/#!topic/mpf-users/4anGZjhW7i4) (backport)

## Documentation

No changes

# Dev release (future 0.51)

We pushed MPF 0.51.0-dev-11 and MPF-MC 0.51.0-dev.2.

## Changes/New features

* [Support other channel orders than RGB for all RGB DMDs](https://github.com/missionpinball/mpf-mc/issues/345) - jab based on [request from Cadrion](https://groups.google.com/forum/#!topic/mpf-users/1EtJxmAZiow)
* [Prevent warnings during init and batch incandescant update for OPP](https://github.com/missionpinball/mpf/pull/1220) - jab
* [Improve FAST behaviour during MPF init](https://github.com/missionpinball/mpf/pull/1221) - jab
* [Entrance switch ignore window](https://github.com/missionpinball/mpf/pull/1216) - avanwinkle
* [Improved README.md for the MPF project](https://github.com/missionpinball/mpf/pull/1219) - austinbgill
* [Update kivy to version 1.10.1](https://github.com/missionpinball/mpf-mc/pull/346) - jab
* [Prevent bad switch config for drop_targets, shots and autofires](https://github.com/missionpinball/mpf/pull/1227) - jab

## Bugfixes

* [Fix mode events when starting/stopping mode from BCP](https://github.com/missionpinball/mpf/issues/1215) - jab based on [report by Travis Martin](https://groups.google.com/forum/#!topic/mpf-users/u48fOP3TIx0)
* [Fix display_light_player crash when used in mode](https://github.com/missionpinball/mpf/pull/1224) - jab
* [Fix crash in BCP with MPF Monitor](https://github.com/missionpinball/mpf/pull/1226) - jab based on [report from alex](https://groups.google.com/forum/#!topic/mpf-users/4anGZjhW7i4)

## Documentation

* [Document appliance classes and common ground](https://github.com/missionpinball/mpf-docs/commit/44c15465db97108d93fad1637c43a3778afdd4aa) - jab
* [Added examples for PD-LED](https://github.com/missionpinball/mpf-docs/commit/a57ddb305abf8b4738e355143be1222d6c763b6b) - jab
* [Improved bonus mode documentation](https://github.com/missionpinball/mpf-docs/pull/173) - avanwinkle
* [Document ball and game end mode blocking](https://github.com/missionpinball/mpf-docs/commit/fd7112356a26413abe27a0e0cb3980f586f3a6c9) - jab inspired by Lynn
* [Extra ball based on score example](https://github.com/missionpinball/mpf-docs/commit/2d8e6b7d073f6904564896ca485b3f3c69951027) - jab based on [example from Lynn](https://groups.google.com/forum/#!topic/mpf-users/cOQKDQIIu-g)
* [How to use high score mode in EMs](https://github.com/missionpinball/mpf-docs/commit/318541ee4349776e5fb4660fcd44b29104f1a842) - jab based on [example from Lynn](https://groups.google.com/forum/#!topic/mpf-users/cOQKDQIIu-g)
* [Document RGB DMD channel_order parameter](https://github.com/missionpinball/mpf-docs/commit/a21bcae7b7be032c918a987fdb32cda8ee2a567e) - jab
* [Added example of game mode which increases multiplier when lanes are complete](https://github.com/missionpinball/mpf-docs/pull/176) - travisbmartin
* [No longer claim Python 3.4 support - it is EOL](https://github.com/missionpinball/mpf-docs/commit/1639e5b62f221b6a525b3ca39da6b68dd2d88752) - jab
* [Document PC power on/off](https://github.com/missionpinball/mpf-docs/commit/8bb7de3ce54153c8e7afbc3fdb992b13bb000409) - jab
* [Typos](https://github.com/missionpinball/mpf-docs/pull/177), [Typos](https://github.com/missionpinball/mpf-docs/pull/178) - travisbmartin 
* [Improve skill shot example to prevent race condition and add timeout](https://github.com/missionpinball/mpf-docs/commit/063dd00c2b9f0db50b099528e3f2d948c7e40f28) - jab based on [question from mike wiz](https://groups.google.com/forum/#!topic/mpf-users/Fxuh95wxmjY) 
* [Document scoring based on logic blocks](https://github.com/missionpinball/mpf-docs/commit/a843d366bed107544aebf2198f80f07a501adb5b) - jab based on [question from alex](https://groups.google.com/forum/#!topic/mpf-users/3mShvjtjfPU)
* [Describe how to debug crashes with GDB](https://github.com/missionpinball/mpf-docs/commit/27a7c31b524f2a1890c97e6dbc86e08811e31e38) - jab
* [How to tune eject_timeouts in ball devices](https://github.com/missionpinball/mpf-docs/commit/ec7477e5a9c3e03adf24473599c2c2909db0a75a) - jab
* [Understanding tags in MPF](https://github.com/missionpinball/mpf-docs/pull/179) - cfbenn
* [Example for using MC with multiple screens](https://github.com/missionpinball/mpf-docs/commit/2d62878bc2a04d699e81fd12fad77d1ad4b13a52) - jab based on example from Brian Cox/cfbenn/qcapen

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [New OSC module](https://github.com/missionpinball/mpf/pull/1200) - jab
* [P-Roc libpinproc in separate thread (since it is currently blocking)](https://github.com/missionpinball/mpf/pull/1195) - jab
* [Change sound volume handling in sound_player/sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen

## Upcoming changes/Not landed yet

* [Support for the Pololu Tic stepper controller](https://github.com/missionpinball/mpf/issues/1217) - wolfmarsh
* [Support for LISY35](https://github.com/missionpinball/mpf/issues/1218) - jab

## New contributors

Welcome travisbmartin and austinbgill!

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
