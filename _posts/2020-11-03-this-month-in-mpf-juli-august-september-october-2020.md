---
layout: post
author: jab
title: This Month in MPF Juli, August, September and October 2020
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in MPF Juli, August, September and October  2020?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Hyperdrive]({% link _projects/hyperdrive.md %})
* [Kraken]({% link _projects/kraken.md %})
* [Pinbot Extended]({% link _projects/pinbot_extended.md %})
* [William's Grand Prix Conversion]({% link _projects/williams_grand_prix_conversion.md %})
* [Zaccaria Combat Conversion]({% link _projects/zaccaria_combat_conversion.md %})
* [Flash Remake]({% link _projects/flash_remake.md %})
* [Holopin]({% link _projects/holopin.md %})
* [Daftpunk]({% link _projects/daftpunkt.md %})
* [Supernatural]({% link _projects/supernatural.md %})
* [Attack From Mars From Scratch]({% link _projects/attack_from_mars_from_scratch.md %})
* [Monty Python and The Holy Grail]({% link _projects/monty_python_and_the_holy_grail.md %})
* [Tron 1982]({% link _projects/tron_1982.md %})
* [Peanuts]({% link _projects/peanuts.md %})
* [Cuphead]({% link _projects/cuphead.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anything wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.53 release

We released MPF 0.53.3 and MPF-MC 0.53.5.

## Bugfixes

* No changes

# Dev release (future 0.54)

We pushed MPF 0.54.0-dev.78 and MPF-MC 0.54.0-dev.20.

## Changes/New features

* [Add source_devices to multiball_locks](https://github.com/missionpinball/mpf/commit/20f35f692d2cb7b7d02bf4ab8c5a0c92fd6be08f) - jab
* [Select pulse_ms based on ball count during eject](https://github.com/missionpinball/mpf/pull/1525) - jab
* [Add start_running option to shows](https://github.com/missionpinball/mpf/pull/1524) - avanwinkle
* [Support pulse_power in P/P3-Roc where possible](https://github.com/missionpinball/mpf/commit/d08885983bbbfd23e92ae9061d44651481801ac6) - jab
* [Better log output for P/P3-Roc](https://github.com/missionpinball/mpf/commit/1c6df104f222be640934d01a7e9cefaa282d26db) - jab
* [Always log OPP chain serial](https://github.com/missionpinball/mpf/commit/c32220ea0139d62ccbd3fa10b9d4519cb4cf6ec7) - jab
* [Support GPIO inputs on P3-Roc](https://github.com/missionpinball/mpf/commit/a07e4a26863c85fc8cbe82a6ae6f6581bff5e314) - jab
* [Faster and better light batching](https://github.com/missionpinball/mpf/commit/e4c7355544ddc04fb5364fc9f53af14dde3c6ca1) - jab
* [Support Neopixel Wings on OPP](https://github.com/missionpinball/mpf/commit/de1b6f24b7543e945fe1fad65dc627c07e302e36) - jab
* [Prevent fades to the previous color](https://github.com/missionpinball/mpf/commit/80d2c9247634248c4995fab4e281ab43c5228c75) - jab
* [Deterministic fades](https://github.com/missionpinball/mpf/commit/d5bf5923be7d45d4b6594ac72ca556c19cf7b9fe) - jab
* [Allow platforms to set batch granularity for fades](https://github.com/missionpinball/mpf/commit/9418baeada0912060644d4c9dc5c61125f027da0) - jab
* [Improve ball counters](https://github.com/missionpinball/mpf/pull/1527) - jab
* [Python 3.8 compatibility (only MPF not MC because of kivy)](https://github.com/missionpinball/mpf/commit/264b0dc9e25b74526a7521facefd74f5eb60b338) - jab
* [Support Repulse on EOS in MPF (only supported in Spike so far)](https://github.com/missionpinball/mpf/commit/64b60e0777d7ff3b03a44bd86d97d1036903ff88) - jab
* [Event to reset high scores](https://github.com/missionpinball/mpf/commit/b89543732f6d051234dcf99eb8e0a014ac2e74c2) - jab
* [Event to reset audits](https://github.com/missionpinball/mpf/commit/5a07acaa3fac8330f1ef60d27d200350c585e34c) - jab
* [Event to reset earnings records](https://github.com/missionpinball/mpf/commit/cdfe1b5076bae28b5ba776b2d4754e73b69227a2) - jab
* [Event to reset credits](https://github.com/missionpinball/mpf/commit/52453e29fb064c0509d19503f62b7b5dea56d52d) - jab
* [More modern service mode](https://github.com/missionpinball/mpf/commit/2c689a7e0fe04c47f60aa65a5bae42b3b3d36322) - jab
* [Add twitch bot support](https://github.com/missionpinball/mpf/pull/1530) - Mark Seiden
* [Improve twitch bot](https://github.com/missionpinball/mpf/pull/1531) - Mark Seiden
* [Add advance_random_events to accruals](https://github.com/missionpinball/mpf/commit/10f55b2ca93e1ed2bc9c4c547651d48c45bca97d) - jab
* [Show a nice error when communication with P/P3-Roc breaks down](https://github.com/missionpinball/mpf/commit/f01f9da7595db4440135d0c77c581951b4fc0da6) - jab
* [Support more than 256 lights in LISY API > 10](https://github.com/missionpinball/mpf/commit/4f9c04d357db47e586d051e8823e1d31f65f2059) - jab
* [Extend motor device](https://github.com/missionpinball/mpf/commit/2bcd15d42148e62bcc9d048e502b24f80a2ed48b) - jab
* [Add shop jump](https://github.com/missionpinball/mpf/pull/1532) - avanwinkle
* [Add settle_time_ms to entrance switch counter to prevent ejecting thin air](https://github.com/missionpinball/mpf/commit/78d5790f7c37b1c96844c002a918463cada3246d) - jab
* [First version of VPE platform (not finished yet)](https://github.com/missionpinball/mpf/commit/c1742f36ef714c7783250313b8bb51644f34d2f4) - jab
* [Test and build on Ubuntu 20.04](https://github.com/missionpinball/mpf/pull/1534) - jab
* [Support conditional events and fallback for random_event_player](https://github.com/missionpinball/mpf/pull/1536) - avanwinkle
* [Python 3.8 support in MPF-MC (except kivy)](https://github.com/missionpinball/mpf-mc/commit/10bed3e964f9ad2d44b8d481e10e95609584feae) - qcapen
* [Faster image loading in sequences](https://github.com/missionpinball/mpf-mc/commit/4d866b929caf59efe7a87a8814fa05fa144e8937) - jab
* [Add block events to text_input and use them in carousel](https://github.com/missionpinball/mpf-mc/pull/406) - avanwinkle
* [Nicer errors in MC](https://github.com/missionpinball/mpf-mc/pull/408) - avanwinkle
* [Expose switch config in pypinproc](https://github.com/missionpinball/pypinproc/pull/6) - jab
* [Support loading light shapes from MPF Monitor in showcreator](https://github.com/missionpinball/showcreator/commit/06f712161b77ae34f1095ad9bc5ecf173a187267) - markinc
* [Add Mac build for showcreator](https://github.com/missionpinball/showcreator/commit/4c411ef810a36f6e5a2c207b0cb6cdc891b5b72b) - markinc
* [Improve logging in MPF Spike Bridge](https://github.com/missionpinball/mpf-spike/commit/e4fa12564954672f83fe9c4ba4299c54c0c26e9e) - jab
* [Extend MPF Monitor with a lot of new features](https://github.com/missionpinball/mpf-monitor/pull/29) - kylenahas
* [Monitor performance improvements](https://github.com/missionpinball/mpf-monitor/commit/2ad4b836cb483e5b4b8e74a395b0a913a8647867) - kylenahas
* [More monitor perf improvements](https://github.com/missionpinball/mpf-monitor/commit/26fe7e016b5232bfa0856b27cc3df93ced5f5a50) - jab
* [Add config arg to MPF Monitor](https://github.com/missionpinball/mpf-monitor/pull/32) - avanwinkle

## Bugfixes

* [Fix crash when a ball is lost (because of the next bug)](https://github.com/missionpinball/mpf/commit/e249fde9c05b8f3b85549154ddbc14387e8a977b) - jab
* [Prevent ball skipping when target is not a ball device](https://github.com/missionpinball/mpf/commit/e0fd2a8e73cf15bab859baa58e281df33a2acd1d) - jab
* [Consistent jam switch handling in ball counter](https://github.com/missionpinball/mpf/commit/54557df2a8b36cfae22823b5d09b8da19ab3f61c) - jab
* [Prevent incorrect playfield activation by drop_target_bank resets](https://github.com/missionpinball/mpf/commit/e361a9f55275af2d276cd0bb854f043794d7e9da) - jab
* [Fix light ordering for fades](https://github.com/missionpinball/mpf/commit/921df14f5a76f47064fb359ed3f4274ee4157199) - jab
* [Fix config parsing for developers.missionpinball.org](https://github.com/missionpinball/mpf/commit/19fcb85b89942b1fbc9d361ca77097c6ee403671) - jab
* [Use the correct commands for the correct Spike Firmare (Spike System 1 vs System 2)](https://github.com/missionpinball/mpf/commit/61568f61ff478600adde707cfd775c1ba13e2cbd) - jab
* [Correct Active Mode Updates to MPF Monitor](https://github.com/missionpinball/mpf/commit/8721af79f4a5fdbe150889b9f16dd8ea7b842453) - jab
* [Fix config validation issues with System 11](https://github.com/missionpinball/mpf/commit/7b3896967eb185a460e74796ac5fc95d42f89b6a) - jab
* [Fix potential crash](https://github.com/missionpinball/mpf/commit/ed647d6627e77b842daad6359b5665523a418daa) - jab
* [Always configure both banks of all PD-16s on P/P3-Roc to prevent polarity issues and stuck on coil on the hardware](https://github.com/missionpinball/mpf/commit/867e4109e43a5317d6d7ec488cec627537aa7945) - jab
* [Fix sound loop bug](https://github.com/missionpinball/mpf-mc/commit/dafc8c0517c9af2eaa78fb652b17577b496d4552) - qcapen
* [Fix loop bug when stealing/replacing a playing sound with a higher priority sound](https://github.com/missionpinball/mpf-mc/commit/02e85e00e3adddeb08b482618ae9fbad1f0d5072) - qcapen
* [Fix animations when two slides animate the same image](https://github.com/missionpinball/mpf-mc/commit/ef02a5aaf793620b5ea1fdcce8282ef54ba4d923) - jab
* [Do not crash on empty config collections](https://github.com/missionpinball/mpf-mc/commit/24f19f6485760eb9f1af56e97d7f0cd5ca7f8dd9) - jab
* [Fix animations in slides in shows](https://github.com/missionpinball/mpf-mc/commit/37479c026d56bf079663676e3b3330ca5f70c914) - jab
* [Prevent crash in sound_player with placeholders](https://github.com/missionpinball/mpf-mc/commit/d7b214f0f440c8227e1b9f31ec07c52b34844059) - jab
* [Expose video control events to MPF](https://github.com/missionpinball/mpf-mc/commit/37371a09565e83c2cba2456edf5eff5fc2deadfd) - jab
* [Fix crashes in image pool and regression test them](https://github.com/missionpinball/mpf-mc/commit/685fbd74caa2c215f029b0f02a3f11325940b599) - jab
* [Fix Spike 2 Init Sequence](https://github.com/missionpinball/mpf-spike/commit/88b592129202258e6aa338ec2e854217656bce3c) - jab
* [Fix incorrect active modes in MPF Monitor](https://github.com/missionpinball/mpf-monitor/commit/463ac293f2930658a36ee41d84af213b879541e7) - jab
* [Prevent crash in Monitor](https://github.com/missionpinball/mpf-monitor/commit/ef9954c922d4f175d00624d1314d5ae8a9b83dcc) - jab

## Documentation

* [How to wire coils and scoops](https://github.com/missionpinball/mpf-docs/commit/f4cbfdee80daa2584b17537550e8080b200df895) - jab
* [Magnet example](https://github.com/missionpinball/mpf-docs/commit/5f4e518ab9e746a8973414c05528cb6d9d5cacc0) - jab
* [How to debug MPF Spike Bridge](https://github.com/missionpinball/mpf-docs/commit/a8caf3be0663ec1d6b81a3c2ea13f700932ba3f4) - jab
* [Add Physical Building Section](https://github.com/missionpinball/mpf-docs/commit/d359cb24a19252331fe6f925fbe59cc9fce0603e) - Nate
* [Add Stern Magnet Board](https://github.com/missionpinball/mpf-docs/commit/70f1b75c76e3c148aaf4187a19780b6afd1f2b86) - jab
* [Document start_running in shows (with examples)](https://github.com/missionpinball/mpf-docs/pull/321) - avanwinkle
* [How to capture spike net bus](https://github.com/missionpinball/mpf-docs/commit/687d532d59e67f524e013d660bff92f9c0c194c2) - jab
* [How to replace FETs on FAST hardware](https://github.com/missionpinball/mpf-docs/commit/856a22769334392d4a7fc4b6e61332fa33bc231e) - jab
* [Dedicated Magnet Driver boards](https://github.com/missionpinball/mpf-docs/commit/078aba3da5f8bc2ef98af53c892541433f80fa13) - jab
* [Fix typos](https://github.com/missionpinball/mpf-docs/pull/322) - bghill
* [Update Windows Install Instruction for Multimorphic](https://github.com/missionpinball/mpf-docs/commit/7165f0d25ce7a823b91c1aa03c8b30285d23b581) - qcapen
* [Add part numbers](https://github.com/missionpinball/mpf-docs/pull/324) - bghill
* [Fix snux docs](https://github.com/missionpinball/mpf-docs/commit/825b0d46573318fe633a56543c7cf1fc6efcacb3) and [more](https://github.com/missionpinball/mpf-docs/commit/ea8092edb2bab3dacc6b47c53d325d96eb08094a) - jab
* [Remarks on referencing slides in a show from outside](https://github.com/missionpinball/mpf-docs/commit/68ae1aa90c2b1051a588ff6b0f64fc4512357866) - jab
* [Document twitch bot](https://github.com/missionpinball/mpf-docs/pull/326) - Mark Seiden
* [Add details about keys and widgets](https://github.com/missionpinball/mpf-docs/pull/327) - atummons
* [Enhance twitch docs](https://github.com/missionpinball/mpf-docs/pull/328) - Mark Seiden
* [Document known P/P3-Roc errors](https://github.com/missionpinball/mpf-docs/commit/ceefc644aff087902459fc9ed2b0b5b255c2443b) - jab
* [Link correct demo man from docs](https://github.com/missionpinball/mpf-docs/commit/53adb1560264d2cce3a451b0d4c6d847f90bd8c3) - jab
* [Document common demo man issues](https://github.com/missionpinball/mpf-docs/commit/f976589627ea4250372442893569338dff4a5e43) - jab
* [Document advance_random_events](https://github.com/missionpinball/mpf-docs/commit/41b6e18f177c931c0ec0f3c6c365e1ae2cdebc45) - jab
* [Document reset_audit_events](https://github.com/missionpinball/mpf-docs/commit/969a7aff38ddc66b06d2226649f6ac09490cb3b5) - jab
* [Document repulse on EOS for flippers](https://github.com/missionpinball/mpf-docs/commit/fda9e5110eceb77beea9699769f71a34f6842d52) - jab
* [Document reset_high_score_events](https://github.com/missionpinball/mpf-docs/commit/75663630de715bd76b0e00e82d51bbce727dc792) - jab
* [Document light chaining with previous and start_channel](https://github.com/missionpinball/mpf-docs/commit/120fdb7380f2a9443927fb3d180193f41739da94) - jab
* [Document source_device in multiball_locks](https://github.com/missionpinball/mpf-docs/commit/656139882a753ce6293ab6bc0fd0981b2e1e1dc6) - jab
* [Update Motor documentation](https://github.com/missionpinball/mpf-docs/pull/330) - Lance-o-nator
* [Improve tutorial](https://github.com/missionpinball/mpf-docs/pull/331) - flamtime
* [Add driver troubleshooting](https://github.com/missionpinball/mpf-docs/commit/ce47545593cd1fb313254b305cd1311cc496425f) - jab
* [Document P/P3-Roc runtime errors](https://github.com/missionpinball/mpf-docs/commit/8fb185fb35a3dbdcd42bc7c369a63671f8137a62) - jab
* [P/P3-Roc Firmware Upgrade section](https://github.com/missionpinball/mpf-docs/commit/79323b28ed2a6b4dc558c44468bbdd2bb58bbb62) - jab
* [Document CobraPin platform](https://github.com/missionpinball/mpf-docs/pull/335) - cobra18t
* [Fix reset_when_complete in docs](https://github.com/missionpinball/mpf-docs/pull/338) - avanwinkle
* [Document carousel block_events](https://github.com/missionpinball/mpf-docs/pull/337) - avanwinkle
* [Document more common errors](https://github.com/missionpinball/mpf-docs/commit/17e2d6f929458e0ec88d2aef5c74c90b1ca9cc6f) - jab
* [More breakout boards](https://github.com/missionpinball/mpf-docs/commit/fdef70e5717982717ac2fd0147c42cfe762af84e) - jab
* [Ubuntu 20.04 install instructions](https://github.com/missionpinball/mpf-docs/commit/1172899a058fb728ccd68acadd11362274eeb087) - jab
* [Add missing config references for release](https://github.com/missionpinball/mpf-docs/pull/339) - avanwinkle
* [Renamed end_loop_at and start_loop_at to loop_end_at and loop_start_at](https://github.com/missionpinball/mpf-docs/commit/2ec8a3b7c33ace4ec92023e3c10423663a410bcc) - qcapen

Have a look at the [dev documentation](https://docs.missionpinball.org/en/dev/).
Do you have an example which is missing there? Please send it to us!

## Open PRs/Not landed yet

* [Multiply volumes instead of overwriting them in sound_player and sound_loop_player](https://github.com/missionpinball/mpf-mc/pull/333) - qcapen (breaking change)
* [Multi display updates improvements](https://github.com/missionpinball/mpf-mc/pull/323) - qcapen

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

Welcome flamtime, cobra18t, Lance-o-nator and bghill!

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
