---
layout: post
author: jab
title: This Month in MPF February 2020
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in February 2020?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Dealers Choice Revived]({% link _projects/dealers_choice.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anthing wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.53 release

We released MPF 0.53.2 and MPF-MC 0.53.1.

## Bugfixes

* [Fix master volume bug](https://github.com/missionpinball/mpf-mc/commit/8aab379b5b8c05132dd12f4b106b11edb5ae5a4a) - qcapen

# Dev release (future 0.54)

We pushed MPF 0.54.0-dev.7 and MPF-MC 0.54.0-dev.2.

## Changes/New features

* [Better default logging for ball devices](https://github.com/missionpinball/mpf/commit/22efb222f7b09a7dbd2d77590d444790d324b04e) - jab
* [Support event args in show_tokens](https://github.com/missionpinball/mpf/pull/1492) - jab
* [Log virtual time in unit tests](https://github.com/missionpinball/mpf/commit/5e3c61527607c863193410567385e78657e2755f) - jab
* [New `mpf format` command to format configs](https://github.com/missionpinball/mpf/pull/1499) - jab
* [Refactor hardware fades for performance](https://github.com/missionpinball/mpf/pull/1489) - jab
* [Driverboards per platform to support FAST and P-Roc in parallel in one machine](https://github.com/missionpinball/mpf/commit/3372fdfcfa57029fcc2803090151e829066f7af9) - jab
* [Crash asset loader thread on exception](https://github.com/missionpinball/mpf-mc/commit/c3d3116846bfc20ba16e53df10a6bfba1360b6dc) - jab
* [Validate widgets and targets in slide_player](https://github.com/missionpinball/mpf-mc/commit/d269acd57a2ee09f65c53c83c674cfa345e00c9a) - jab
* [Validate slides in widget_player](https://github.com/missionpinball/mpf-mc/commit/c458b9e6baa66a9d5aae2298f8fb0a7a81877dda) - jab
* [Refactor pypinproc to use PRWriteDataUnbuffered](https://github.com/missionpinball/pypinproc/commit/a34a26a39a93ca50da92f795f60fa157b5979c2c) - jab
* [Refactor libpinproc to use PRWriteDataUnbuffered](https://github.com/missionpinball/libpinproc/commit/031109f5ecabca594ee934423d4183b82b147f27) - jab
* [Util cleanup](https://github.com/missionpinball/mpf/commit/96b628496d0ff7d01b1c0a36cbefc81931d849dc) - jab

## Bugfixes

* [Fix multiple subscriptions in show_player](https://github.com/missionpinball/mpf/pull/1498) - jab
* [Fix new fades in VPX](https://github.com/missionpinball/mpf/commit/ad71f381ce8a0e65f28958e51cf8a8b38a6154fb) - Wolfmarsh
* [Add test for VPX platform](https://github.com/missionpinball/mpf/commit/c4ecc0bdf23a14bef207234b29053818aac15c7d) - jab
* [Fix multiple subscriptions in light_player](https://github.com/missionpinball/mpf/pull/1500) - jab
* [Fix gamma test slide](https://github.com/missionpinball/mpf-mc/pull/395) - jherrm
* [Add test for gamma_test_slide](https://github.com/missionpinball/mpf-mc/commit/d15a5de4f27124d4b879b24ff94932060a85b3c7) - jab
* [Do not crash test when sound system is not loaded](https://github.com/missionpinball/mpf-mc/commit/9c0889ea6a3a864d941028b2894f385538082c58) - jab
* [Test and fix end_bonus_event](https://github.com/missionpinball/mpf/commit/70ec82cbaf2080bfb4270fe15fde51fe36f38db1) - jab
* [Only validate widgets when using the add action](https://github.com/missionpinball/mpf-mc/commit/9fb8f9a8cf2bfc1df43e626511ee0cb9fdb1d2fa) - jab
* [Fix master volume bug](https://github.com/missionpinball/mpf-mc/commit/834ef2f22c8ef0ffb46cefa62c2db7069681949f) - qcapen

## Documentation

* [Support assets in doc tests](https://github.com/missionpinball/mpf/commit/3aa48cbb120a43a4f2146ecc84965f8ba30d1be6) - jab
* [Support virtual platform in doc test cases](https://github.com/missionpinball/mpf/commit/07084c697831a082edb861b8d0e9f78e517bd713) - jab
* [Document common problems with Numlock when using keyboard in MPF](https://github.com/missionpinball/mpf-docs/commit/11c059708b7f0ea10f35c9377480469d9fea8247) - jab
* [Example for multiball without physical lock](https://github.com/missionpinball/mpf-docs/commit/cd91947067fac439480e4218bd06f3716a31fe7f) - jab
* [Reformat all examples for good copy and paste experience](https://github.com/missionpinball/mpf-docs/pull/274) - jab
* [Extend PD-LED FET documentation](https://github.com/missionpinball/mpf-docs/pull/275) and [drawing](https://github.com/missionpinball/mpf-docs/commit/16c977d1bb491a87772700a8f4ab3cef70925bae) - colemanomartin
* [Test and fix mc examples](https://github.com/missionpinball/mpf-docs/commit/2b5c508dab2d26185f8a3e4706a0a9a8109ab42b), [more](https://github.com/missionpinball/mpf-docs/commit/9992d9cdb9b806ff44285d9de0a9e47172b39655) and [more](https://github.com/missionpinball/mpf-docs/commit/94103178f53c7bb9bcb52c3efd8bcfbb31adb8f4) - jab
* [Test all slides in the tutorial](https://github.com/missionpinball/mpf-docs/commit/abf83cf4a82d70b523a160b9044da10094c0ace9) - jab
* [Improve PD-LED documentation](https://github.com/missionpinball/mpf-docs/pull/277) - seanirby
* [Fix typo](https://github.com/missionpinball/mpf-docs/pull/276) -  driskel
* [Fix settings name](https://github.com/missionpinball/mpf-docs/pull/278) - enteryourinitials
* [Update docs for driverboards per platform](https://github.com/missionpinball/mpf-docs/commit/90536596cf3c123a462e046a5d17af332754ff39) - jab
* [Test and fix DMD style names in examples](https://github.com/missionpinball/mpf-docs/commit/b518aafac200b76e3e08ce0eed542921f346d858) - jab
* [Test and fix all kinds of slightly broken examples](https://github.com/missionpinball/mpf-docs/commit/784e2bd9fa2ca09784533e79654caea11806eb34) - jab
* [Test and fix animation examples](https://github.com/missionpinball/mpf-docs/commit/a3e880ab5ca5d52bfe9a99e8bcb0d17f9c5f5191) - jab
* [Test and fix widget examples](https://github.com/missionpinball/mpf-docs/commit/74323c7bad7a962900cd422d41ed6f860c6db92e), [more](https://github.com/missionpinball/mpf-docs/commit/6813770613ac5b528a6e368fe884604b4ab2992e) and [more](https://github.com/missionpinball/mpf-docs/commit/8a35363399e1bdfb63ea6310246799e7dbd0fc0f) - jab
* [Test and fix slide examples](https://github.com/missionpinball/mpf-docs/commit/6d03831c3afb829a649c78c3cde99e5b449579b7) and [more](https://github.com/missionpinball/mpf-docs/commit/90532067b40f8f39004cff98c36b340b9e0640b4) - jab
* [Test and fix display examples](https://github.com/missionpinball/mpf-docs/commit/2a07d6b4eac213be57c17e3f6254851d7e497cec) - jab
* [Test remaining mc examples](https://github.com/missionpinball/mpf-docs/commit/bb20f9af918cfb194491da01d5502b666278f847) - jab
* [Add dual_wound_coil example for diverters](https://github.com/missionpinball/mpf-docs/pull/279) - SwizzleFish
* [Document solution for common Windows install problem](https://github.com/missionpinball/mpf-docs/pull/280) - AdrianD72
* [Add mystery award example](https://github.com/missionpinball/mpf-docs/pull/281) - aaronmatthies
* [Fix broken links and references to ball_locks](https://github.com/missionpinball/mpf-docs/pull/282) - aaronmatthies
* [Link to APC video](https://github.com/missionpinball/mpf-docs/commit/96a68dc656008059977956371dd20969aac68f9f) - jab
* [Remove old-syntax list examples from docs](https://github.com/missionpinball/mpf-docs/commit/27a111e0c861a0923c7a6f2d6d87962488960f9b) - jab
* [Use commas to separate lists](https://github.com/missionpinball/mpf-docs/commit/78eef6b67375dfb14ec8e130aa20be155f7f4c11) - jab

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

Welcome jherrm, enteryourinitials and AdrianD72.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
