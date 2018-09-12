---
layout: post
author: jab
---
What happened in MPF-land in September 2018?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

We are currently preparing for the 0.51 release which will not require
migrations for most users (unless you are using accelerometers).
You might have to run minor cleanups if you are using non-functional/noop
options (such as width on images) which have been removed.
Besides that 0.51 should bring major performance improvements around switches
and event handling.
Furthermore, we improve the error/logging output and added a new production
flag which optimizes the behaviour for unattended operations.

# Current stable release (0.50)

We released MPF 0.50.14 and MPF-MC 0.50.8 with bugfixes and backports.

## Changes

* []()

## Bugfixes

* [Fix mode events when starting/stopping mode from BCP](https://github.com/missionpinball/mpf/issues/1215) - jab based on report by Travis Martin

## Documentation

* []()

# Dev release (future 0.51)

We pushed MPF dev-2.

## Changes/New features

* [Support other channel orders than RGB for all RGB DMDs](https://github.com/missionpinball/mpf-mc/issues/345) - jab based on request from Cadrion

## Bugfixes

* [Fix mode events when starting/stopping mode from BCP](https://github.com/missionpinball/mpf/issues/1215) - jab based on report by Travis Martin

## Documentation

* [Document appliance classes and common ground](https://github.com/missionpinball/mpf-docs/commit/44c15465db97108d93fad1637c43a3778afdd4aa) - jab
* [Added examples for PD-LED](https://github.com/missionpinball/mpf-docs/commit/a57ddb305abf8b4738e355143be1222d6c763b6b) - jab
* [Improved bonus mode documentation](https://github.com/missionpinball/mpf-docs/pull/173) - avanwinkle
* [Document ball and game end mode blocking](https://github.com/missionpinball/mpf-docs/commit/fd7112356a26413abe27a0e0cb3980f586f3a6c9) - jab inspired by Lynn
* [Extra ball based on score example](https://github.com/missionpinball/mpf-docs/commit/2d8e6b7d073f6904564896ca485b3f3c69951027) - jab based on example from Lynn
* [How to use high score mode in EMs](https://github.com/missionpinball/mpf-docs/commit/318541ee4349776e5fb4660fcd44b29104f1a842) - jab based on example from Lynn
* [Document RGB DMD channel_order parameter](https://github.com/missionpinball/mpf-docs/commit/a21bcae7b7be032c918a987fdb32cda8ee2a567e) - jab

Have a look at the [dev documentation](http://docs.missionpinball.org/en/dev/).

## Open PRs/Not landed yet

* [New OSC module](https://github.com/missionpinball/mpf/pull/1200) - jab
* [P-Roc libpinproc in separate thread (since it is currently blocking)](https://github.com/missionpinball/mpf/pull/1195) - jab
* [Entrance switch ignore window](https://github.com/missionpinball/mpf/pull/1216) - avanwinkle
* [Change sound volume handling in sound_player/sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen

## Upcoming changes

* [Support for the Pololu Tic stepper controller](https://github.com/missionpinball/mpf/issues/1217) - wolfmarsh
* More stepper and servo hardware - jab
* Moving slides/widget management to MPF from MPF-MC to improve the programming interface - jab


Did we forget anything? Please let us know.
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
