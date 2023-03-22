---
layout: post
author: jab
title: This Month in MPF April, May and June 2020
tags: [this_month_in_mpf_land, MPF]
---
What happened in MPF-land in April, May and June 2020?
This post will highlight changes in MPF, MPF-MC, MPF monitor, documentation
and the rest of the ecosystem.

# MPF Projects

We collect a list of [active publicly documented projects by MPF users]({% link projects.html %}).
Some new projects which joined the list this month:

* [Haunted House Remake]({% link _projects/haunted_house_remake.md %})
* [DEVO Pinball]({% link _projects/devo.md %})

We know that there are a lot more projects.
Let us know if you want to be listed here as well (it does not matter in which
stage your project is).
If we got anything wrong or your project has been finished in the meantime
please tell us as well and we will update your entry.

# 0.53 release

We released MPF 0.53.3 and MPF-MC 0.53.5.

## Bugfixes

* [Fix mac build issues](a5cca967c83c035da325fc35b2175f55d3b4d689) - qcapen (backport)
* [Fix entrance_switch crash in smart_virtual](d83b83e3fd38b21eb8705e75921eda11d2db5761) - jab (backport)

# Dev release (future 0.54)

We pushed MPF 0.54.0-dev.50 and MPF-MC 0.54.0-dev.7.

## Changes/New features

* [Better error messages for incorrectly formatted shows](https://github.com/missionpinball/mpf/commit/6c4878cfa4fc3b56c3eb68e04137a881b259a450) - jab
* [Retry connect to LISY/APC serial](https://github.com/missionpinball/mpf/commit/b5549ca2084734abc47c310ae3965106160e7129) - jab
* [Validate shows in achievements](https://github.com/missionpinball/mpf/commit/e89e71d18968f6f744c633b9ceb261a46d03bd42) - jab
* [Improve smart_virtual errors](https://github.com/missionpinball/mpf/commit/cfb5467351f7ad2880a6560f8828a08ef67169af) - jab
* [Improve error when a required setting is missing](https://github.com/missionpinball/mpf/commit/4d95608d06091909c0fbbf9f1da2c40659756958) - jab
* [Improve generic validator errors](https://github.com/missionpinball/mpf/commit/27d337f67adaac2a15d7d6409770c11507aab4fd) - jab
* [Support switches in OSC platform](https://github.com/missionpinball/mpf/commit/723de4b177de3fb9ff2fc2768108668a555c25df) - jab
* [Implement events in OSC platform](https://github.com/missionpinball/mpf/commit/c19b087764592b7d342ec4d49bb792c359f8a49c) - jab
* [Support BCD, 14-segment and 16-segment displays as segment_display](https://github.com/missionpinball/mpf/commit/22827621831d34dc9397ebdc0898602d8f698b73) - jab
* [Improve empty device collection error](https://github.com/missionpinball/mpf/commit/5a6ae34d4763bcb3e4bbc82f764f9f3787bcb677) - jab
* [Validate playfield_active tags on shot switches](https://github.com/missionpinball/mpf/commit/2a6615cf80bb8c09ec2823816db4d115d63eb2d5) - jab (breaking change - you have to remove those tags)
* [Point users to our fork of apigpio (called apigpio-mpf)](https://github.com/missionpinball/mpf/commit/bd05b7531568a7e6213a6b5e5583d05f37760038) - jab
* [Validate platforms and prevent configuring features which do not exist on platform](https://github.com/missionpinball/mpf/commit/938a678c216390794ac20ae2bfd2f470d29a0761) - jab
* [Runtime errors with documentation links](https://github.com/missionpinball/mpf/commit/8132de4f18ffcc03c5ae32eca5e181727d2f6d37) - jab
* [Add glow effect](https://github.com/missionpinball/mpf/pull/1513) and [2](https://github.com/missionpinball/mpf-mc/pull/400) - seanirby (see blog post about glow effect)
* [Add font for 14-segment displays similar to Williams System 11 displays](https://github.com/missionpinball/mpf-mc/pull/399) - seanirby
* [Pin all dependencies](https://github.com/missionpinball/mpf/commit/07d49d17945e6b307f853ea583b1ca1401918772) - jab
* [Commandline config generator](https://github.com/missionpinball/mpf/pull/1514) - F4b1-
* [Add end_ball and end_game events to game](https://github.com/missionpinball/mpf/commit/8f23cc83814bf39e4f8e8ae2daed050ab370b8b3) - jab
* [Prevent true and false in placeholder (use True and False)](https://github.com/missionpinball/mpf/commit/90ac1dee0fcb76c1eea9880fea2563a2437311c1) - jab
* [Expose more P/P3-Roc errors](https://github.com/missionpinball/mpf/commit/8a8348ed66c3c112e767d96edb312cf0f838bcce) - jab
* [mpf hardware scan for LISY](https://github.com/missionpinball/mpf/commit/81f64ca9fea2b53f9cb87ae4e90a8c3aa4aba816) - jab
* [Refactor driver lights to properly encapsulate internals](https://github.com/missionpinball/mpf/commit/8c9b9bdc7960d9bd45aa92a76d69e5ba105084eb) - jab
* [Parallel device initialisation](https://github.com/missionpinball/mpf/commit/6fc6b4a8a512d23d8cc840477181a531f975e152) - jab
* [Implement chained lights](https://github.com/missionpinball/mpf/commit/ae3e322fd25b275abe1f8500c1bc742b6990b655) - jab (see separate blog post)
* [Add spread spectrum modulation (SSM) PWM for fast coil for low-noise hold](https://github.com/missionpinball/mpf/commit/1b7f608a56fd902d6d4cb95edd6d9383c0d8e94c) - jab
* [Improve error message on failed template evaluation](https://github.com/missionpinball/mpf/commit/feb86c8dc5ed3696da82b27f848a123acd4af5c2) - jab
* [Add debug output to state_machines](https://github.com/missionpinball/mpf/commit/fe1fc1c4c469dfb5ae239355df0cb02574a1d589) - jab
* [Better config validator error paths](https://github.com/missionpinball/mpf/commit/6ddc1b731789e437eb776f6ad8899bb650fe8231) - jab
* [Support new templates syntax for all template_str](https://github.com/missionpinball/mpf/commit/ddb54c91c82cd67ab6d77ae03adbd23d5ba85756) - jab
* [Add subscriptions in variable_player](https://github.com/missionpinball/mpf/commit/eda7286918008b67d2b077a66365ced2971fba4d) - jab
* [Pass timestamps from platform for switch changes](https://github.com/missionpinball/mpf/commit/2273b27c371a859c531595839cc6ddfe4fca4dec) - jab
* [Refactor hot switch path for performance](https://github.com/missionpinball/mpf/commit/bd6dc68194e909886ff1c180e346e11874645f4c), [2](https://github.com/missionpinball/mpf/commit/90feacf79b3db24335205d6cc6e6ef5f8141161c), [3](https://github.com/missionpinball/mpf/commit/7d256ad27acd97430caec4791ca22517852b1b81), [4](https://github.com/missionpinball/mpf/commit/8ae14a17cd5b06589efc94a5ec5d83da0276d5ec) - jab
* [Add sound_loop_start_at/end_at](https://github.com/missionpinball/mpf/pull/1517) and [implement them in MC](https://github.com/missionpinball/mpf-mc/pull/403) - qcapen
* [Allow multiple entrance_switches](https://github.com/missionpinball/mpf/commit/376ddf05118bf4f24c033390f50b25b25c7d06c0) - jab
* [Prevent event handler with the same name as switches (to catch common beginner mistakes)](https://github.com/missionpinball/mpf/commit/87b61e04f26e8f683b99a0f5263cce27a3888f3d) - jab (breaking change in theory but unlikely for real machines)
* [Performance improvements](https://github.com/missionpinball/mpf/commit/f023ce2c8ac1d55337c3d64455c0ff1fe120518d) - jab
* [Add show_queues to serialize shows](https://github.com/missionpinball/mpf/commit/ab192b62a398cbba3443bcca25a5ad323a1ec083) - jab
* [Support pinproc in Python 3.7 and 3.8 on Windows](https://github.com/missionpinball/mpf/pull/1520) - qcapen
* [Recompiled pinproc for Python 3.5 and 3.6 on Windows to include recent improvements](https://github.com/missionpinball/mpf/pull/1522) - qcapen
* [Improve memory leak finder](https://github.com/missionpinball/mpf-mc/commit/e95f33e7e7d734142e29efd9b2777cc32aaed25d) - jab
* [Add debug button in iMC](https://github.com/missionpinball/mpf-mc/commit/aa3d54809cbc449cc3f7781057a39bd5c4ace46f) - jab
* [Load named_colors in mc and test them](https://github.com/missionpinball/mpf-mc/commit/1d4d87aaaf6c0594e833e307c4d3851dab9ee759) - jab
* [Require ffpyplayer for all platforms as it seems to solve video issues](https://github.com/missionpinball/mpf-mc/commit/694f356d3d926457423d80ad75ea585e2d18414e) - jab
* [Better type hints in mpf-ls](https://github.com/missionpinball/mpf-ls/commit/a8c496120b0e176fb5f5db4f313adda756facc57) - jab
* [Autocomplete events and go to definition for events](https://github.com/missionpinball/mpf-ls/commit/eec997a618dd5573d1e7f7b4a0a42abff944cd95) - jab
* [Support more events in mpf-ls](https://github.com/missionpinball/mpf-ls/commit/c9413e669d0da64076d08f43a078dbb83fc8f8f6) - jab
* [Install latest kivy in debian installer](https://github.com/missionpinball/mpf-debian-installer/commit/cfd0b5acce2091ea5e0fccd815bb82863d0a19e9) - jab
* [Better error handling in debian installer](https://github.com/missionpinball/mpf-debian-installer/commit/3409ea6c191d13b3bec0ef606971441a80c496d2) - jab

## Bugfixes

* [Fix crash in smart_virtual with entrance_switches](https://github.com/missionpinball/mpf/commit/61be48c2889ef40f238c4baac8c9ab17275424f5) - jab
* [Fix achievement_group auto_select with allow_selection_change_while_disabled](https://github.com/missionpinball/mpf/commit/763c829053795e81874c41dbe4e235718597a295) - jab
* [Fix BCP encoding crash](https://github.com/missionpinball/mpf/pull/1512) - seanirby
* [Remove lower-casing of colors because it breaks placeholders](https://github.com/missionpinball/mpf/commit/d7b10f004326314ac0c8d635c3f148a740bda417) - jab
* [Fix crash in variable_player](https://github.com/missionpinball/mpf/pull/1515) - seanirby
* [Fix non-connected switches for P3-Roc](https://github.com/missionpinball/mpf/pull/1516) - seanirby
* [Fix initial switch state for RPi platform](https://github.com/missionpinball/mpf/commit/ddbf3b90503403c1238b13f8ab9d64331fd55405) - jab
* [Fix OSC crashes with complex event parameters](https://github.com/missionpinball/mpf/commit/2ed0c1cfef573fc82155289e1501bf72f3b66603) - jab
* [Fix ball count in multiball_lock full event with physical_only strategy](https://github.com/missionpinball/mpf/commit/a790768a73dacda5d47af7382ef4bd7fdff6f7fa)
* [Do not poll OPP boards without switches](https://github.com/missionpinball/mpf/commit/4f197927f6001631fc48b703936e7e5bd903f7d5) - jab
* [Fix input mask for OPP Neopixel wings](https://github.com/missionpinball/mpf/commit/4469b2df68b6153a8df321689dc949fd04340dd9) - jab
* [Allow duration for wipe transition](https://github.com/missionpinball/mpf/commit/8eabe07550ebde53a0647c20676f5053c6e9270f) - jab
* [Fix crash when not specifying keep_multiplier in bonus entry](https://github.com/missionpinball/mpf/commit/884bb51826affdd1555df0d22b8f892c1b6bff2b) - jab
* [Fix random argument order in OSC events](https://github.com/missionpinball/mpf/commit/260ed2c0d539fd9c3fcce625c3359b47042775b0) - jab
* [Fix crash in drop_target](https://github.com/missionpinball/mpf/commit/4a3cbc40c82ac60b10fb2cc904fdac70f047779e) - jab
* [Respect switch and coils defaults for autofire rules](https://github.com/missionpinball/mpf/commit/48d237acde07923ba31450733652cbd4c316e5da) - jab
* [Fix init race in steppers](https://github.com/missionpinball/mpf/commit/452f47b387ed49a270aa0302520a968cf1a1e64a) - jab
* [Fix number crash in FAST](https://github.com/missionpinball/mpf/commit/a57ca11a58c2836c8d18c3582c0cea467e96e5ea) - jab
* [Fix late crash during shutdown](https://github.com/missionpinball/mpf/commit/6b5e481336dc5dbf770aa8891484b89ee2dac282) - jab
* [Fix crash in digital_outputs with FAST platform settings](https://github.com/missionpinball/mpf/commit/382ec82098ef63a10e7fe5c50b5e9561de847db7) - jab
* [Consistent fade_out for display_light_player](https://github.com/missionpinball/mpf-mc/commit/3cd123ccff7b30c082e1b757851cb74e3919da02) - jab
* [Fix bash export in installer](https://github.com/missionpinball/mpf-debian-installer/commit/601adce3b28d987de7363c0bc34bb71c911454ca) - jab

## Documentation

* [Fix event annotations](https://github.com/missionpinball/mpf/commit/80e7ec1984fc2b5c9cd762be32b4e74bf36c1835) - jab
* [Remove old section about shot reuse](https://github.com/missionpinball/mpf-docs/pull/290) - seanirby
* [Update config references](https://github.com/missionpinball/mpf-docs/commit/e8e5c40c1af34ea518f11550dd084d740a1eb82b) [for](https://github.com/missionpinball/mpf-docs/commit/9aa4558166cff0b6a35f6547c63d5a20f08c9283) [all](https://github.com/missionpinball/mpf-docs/commit/7155cac0347765cef5e8784b2eb79042b5ad252e) [kinds](https://github.com/missionpinball/mpf-docs/commit/c8a32cc84b14babbb000566e3bf01f3306dea3fd) [of](https://github.com/missionpinball/mpf-docs/commit/c8a32cc84b14babbb000566e3bf01f3306dea3fd) [devices](https://github.com/missionpinball/mpf-docs/commit/ce7798640f4eb6cfec279e3050d9f533a9b05c1e), [5](https://github.com/missionpinball/mpf-docs/commit/1706dfb31f4e64d4455147938d6a8c2abcca3fc6), [6](https://github.com/missionpinball/mpf-docs/commit/8625354fc1ac3d8a9155bb8e1eee49dd744d040f), [7](https://github.com/missionpinball/mpf-docs/commit/90e3327576f34b8bf73f8baff9a059db43f01e28) - jab
* [Document color_correction_profiles](https://github.com/missionpinball/mpf-docs/commit/0a534fa84f3b21cc82ecddd7bbc108407fdadf91) - jab
* [Notes about style for text sizes](https://github.com/missionpinball/mpf-docs/commit/cb9d3d3b4479c67c00dfe5d16e34234ae4fa877d) - jab
* [Update tutorial](https://github.com/missionpinball/mpf-docs/commit/85ac5343b2437c9932e28ec54dca4fc6c5c3e003) - jab
* [Update motors](https://github.com/missionpinball/mpf-docs/commit/07a12b2716be26f10ae3c6385696b51a0a4dae3f) - jab
* [Render nice 404 with helpful links](https://github.com/missionpinball/mpf-docs/commit/0dce069119fd11c902a7bad03532c08861ba9435)  jab
* [Links to list of documented error messages](https://github.com/missionpinball/mpf-docs/commit/4fddb09fb46a50b8847a7bb3647b657147dbdda2) - jab
* [Document show format errors](https://github.com/missionpinball/mpf-docs/commit/b9e8d0b1c2bd1e7566e1e6d66cf33cc8988387ce) - jab
* [More errors and document MPF language server](https://github.com/missionpinball/mpf-docs/commit/ce5e86fa45f9a5c4be641851f2c9a8e8e881c1c2) - jab
* [Update BCP reference](https://github.com/missionpinball/mpf-docs/commit/3e03044076b6c9b5665717aeb1c2650a7c76d638) - jab
* [Update multiball_locks reference](https://github.com/missionpinball/mpf-docs/commit/d3fa3a96a1da32225f8615f87c52a6fb900dfa5b) - jab
* [Update steprocker reference](https://github.com/missionpinball/mpf-docs/commit/c69968ad8ce7b45e2aa548ac9bff830e91be0699) - jab
* [Update achievements reference](https://github.com/missionpinball/mpf-docs/commit/06e815f4811fa32b5a5ffc3bc697f17f0f08f143) - jab
* [Update widget_style reference](https://github.com/missionpinball/mpf-docs/commit/1adbe6704718da38d4ea3f6f332a8b7e6213a2a3) - jab
* [Improve state_machine](https://github.com/missionpinball/mpf-docs/pull/294) - atummons
* [Document common errors](https://github.com/missionpinball/mpf-docs/commit/66fd33e45fc92d689e5bc298644a24ec565d9df0) - jab
* [Update videos reference](https://github.com/missionpinball/mpf-docs/commit/0535c6cdfed11bb7065290b568cffd62d4ac5ff3) - jab
* [Add VPX to tutorial](https://github.com/missionpinball/mpf-docs/commit/8236830f4ffbf78a3de3c5d31c1d5c2c20aabb2f) - jab
* [Document OSC platform](https://github.com/missionpinball/mpf-docs/commit/b6a07513813cadb1ad41c1fb3f1932eff8dc3be8) - jab
* [Update variable_player reference](https://github.com/missionpinball/mpf-docs/commit/b84c3a9741964b5058db3a03ed29b0a8a65eee8b) - jab
* [Update snux reference](https://github.com/missionpinball/mpf-docs/commit/d851f6a7c2affc7368c92cc973027df5de4536f1) - jab
* [Update player_vars and shot_groups reference](https://github.com/missionpinball/mpf-docs/commit/91491002281c022fea07559f697a4f5ebc7f5862) - jab
* [Document light_segment_display](https://github.com/missionpinball/mpf-docs/commit/86a1ba2c3f55ba078b731874f842bb85e7509071) - jab
* [Document WS2812 specifics](https://github.com/missionpinball/mpf-docs/commit/849abf2bad063a77a145d764612fc54ce4556c75) and [similar chips](https://github.com/missionpinball/mpf-docs/commit/fd45c5d77b824b7ca55552adeea339ee9862fb9b) - jab
* [Document CFE-ConfigValidator-4](https://github.com/missionpinball/mpf-docs/commit/a1c6626ff7d9faaa50c14a9f2d1004f8512b7661) - jab
* [Document CFE-ConfigValidator-2](https://github.com/missionpinball/mpf-docs/commit/b74df3e9783e1ac6c6bfc60d3d540ab651307a75) - jab
* [Document CFE-ConfigValidator-1](https://github.com/missionpinball/mpf-docs/commit/5cf6dfb01ab5864486813b9506eaf0acaa856f98) - jab
* [Update logic_blocks reference](https://github.com/missionpinball/mpf-docs/commit/dba88e701f89e607574f66cf6d9d0c60ed417a43) - jab
* [Document CFE-ConfigValidator-12](https://github.com/missionpinball/mpf-docs/commit/843a3403a59bc5a1b014f27edde6f76e9cf141c2) - jab
* [Document CFE-ConfigValidator-13](https://github.com/missionpinball/mpf-docs/commit/cf6dd39964234a0e8c891e1eb472c69d1ec29360) - jab
* [Document CFE-DeviceManager-3](https://github.com/missionpinball/mpf-docs/commit/2efd2868252f28ed4223be866031164d2bbf4f62) - jab
* [Document mpf build production_bundle](https://github.com/missionpinball/mpf-docs/commit/efe48f82220478f4048fca44151480d95097d218) - jab
* [Update track_player reference](https://github.com/missionpinball/mpf-docs/commit/5c95e1c6305569499d82f9601bc549b527eb6f70) - jab
* [Update sounds reference](https://github.com/missionpinball/mpf-docs/commit/d1364fabdd3342dadb03807e22f22c370e7ff026) - jab
* [Improve ball_device reference](https://github.com/missionpinball/mpf-docs/pull/297) - chris20-20
* [Improve switches reference](https://github.com/missionpinball/mpf-docs/pull/298) and [more](https://github.com/missionpinball/mpf-docs/pull/303) - chris20-20
* [Fix typo](https://github.com/missionpinball/mpf-docs/pull/299) and [more typos](https://github.com/missionpinball/mpf-docs/pull/300) - chris20-20
* [Update sound_system reference](https://github.com/missionpinball/mpf-docs/commit/e5c01cf4c54739c6507f34beb046b5cb36eb01fe) - jab
* [Update sound_player reference](https://github.com/missionpinball/mpf-docs/commit/73cc7b15b0d6c664c21757a300dab61825e36fdb) - jab
* [Document defaults in references](https://github.com/missionpinball/mpf-docs/commit/e617856fa8c17724adc0badf25455004dfdd0325) - jab
* [Add links to tutorial](https://github.com/missionpinball/mpf-docs/pull/301) and [more links](https://github.com/missionpinball/mpf-docs/pull/304) - chris20-20
* [Improve tutorial](https://github.com/missionpinball/mpf-docs/pull/306) - chris20-20
* [Improve coil_player documentation](https://github.com/missionpinball/mpf-docs/pull/305/files) - chris20-20
* [Fix LCD width and height](https://github.com/missionpinball/mpf-docs/pull/302) - chris20-20
* [Document MC errors](https://github.com/missionpinball/mpf-docs/commit/fad78e9a7ed972f45d84187878f03816c30e35c6) - jab
* [Fix link in docs](https://github.com/missionpinball/mpf-docs/pull/307) - F4b1-
* [Document glow effect](https://github.com/missionpinball/mpf-docs/pull/308) - seanirby
* [Improve event reference](https://github.com/missionpinball/mpf-docs/commit/7efc50933e2a514f7edfd4992f6f465dbc96ea44) - jab
* [Add physical building section](https://github.com/missionpinball/mpf-docs/commit/f12f61b43e83d2a09a83df0a6afa9e0a4e284383) - jab
* [Improve common ground warning](https://github.com/missionpinball/mpf-docs/commit/2c7b553086f6010e2458d160f4467af2097c72cc) - jab
* [Add common issues section for Multimorphic](https://github.com/missionpinball/mpf-docs/commit/c7541a0362b128eab57db0215e6dc78fb517a34c) - jab
* [Playfield layout considerations from Jimmy](https://github.com/missionpinball/mpf-docs/commit/29debb562cade432b8c2645faf58fa5ac21f48de) - jab (content from Compy)
* [More on common ground from Gerry Stellenberg](https://github.com/missionpinball/mpf-docs/commit/5f7f3a8ebe0938f9799253dfda2ad24f56e594d8) - jab (content from Gerry)
* [Update instructions to build docs locally](https://github.com/missionpinball/mpf-docs/pull/309) - seanirby
* [More playfield layout and images](https://github.com/missionpinball/mpf-docs/pull/310) - Compy
* [Example on how to end a game properly using events](https://github.com/missionpinball/mpf-docs/commit/e1118faf9782d17d18d56eee690f8de5ad736892) - jab
* [More details and considerations on coils](https://github.com/missionpinball/mpf-docs/commit/69d7c26fe34da2aa1a89123f1af3c15afde71a8d) - jab
* [Properly document MPF language server](https://github.com/missionpinball/mpf-docs/commit/781fe031c81c4e2ffa1fdbbb51bbc64e4fcdb73f) - jab
* [Clarify that a RPi is not a pinball controller without further hardware](https://github.com/missionpinball/mpf-docs/commit/d60220ad1775e0c210fa527152eca2b4af197523) - jab
* [Related links for all driver howtos](https://github.com/missionpinball/mpf-docs/commit/5af7347edf393f85f2fb858f1a98fb741a6d90f9) - jab
* [Bring back Indy Lane tutorial from old website](https://github.com/missionpinball/mpf-docs/commit/75a89dffb711ba5e0588fe2527ff273eed13662d) - jab (based on content from Brian)
* [Warn about current Python 3.8 issues](https://github.com/missionpinball/mpf-docs/pull/311) - BENETNATH
* [Fix typo in udevadm command](https://github.com/missionpinball/mpf-docs/commit/0085b87b46cbeeeaf998b90da0a23d1cef7c4c89) - BENETNATH
* [General hardware troubleshooting guide](https://github.com/missionpinball/mpf-docs/commit/47ab01fe091d662b04f0e8bfb341366c9baec2df) - jab
* [mpf hardware scan example for the P-Roc](https://github.com/missionpinball/mpf-docs/commit/c62eb279a826c900b5ed44a42adcd831da9e2e25) - jab
* [Document common P/P3-Roc issues](https://github.com/missionpinball/mpf-docs/commit/1e812fb2287a052e786abe88b9a7e2e13350ad8b) - jab
* [Link troubleshooting section from more places](https://github.com/missionpinball/mpf-docs/commit/e4d95a008c069a88a55ea589c7c0e32ea13d0f98) - jab
* [Troubleshooting guide for FAST hardware](https://github.com/missionpinball/mpf-docs/commit/59ed857d8a658c1994e157367b799d8347cd6e81) - jab
* [Correct addressing section for P3-Roc](https://github.com/missionpinball/mpf-docs/commit/db72b53bc013574e616b649b22a93a54ba2f6097) - Coleman
* [More hardware troubleshooting for P3-Roc boards and cables](https://github.com/missionpinball/mpf-docs/commit/1c89200cd2548c8803c594bfec41ce19bc6916c0) - Coleman
* [Document new game events](https://github.com/missionpinball/mpf-docs/commit/4cc8ca2a127093122c3e9a091fadac74c929c495) - jab
* [Document -t command line option](https://github.com/missionpinball/mpf-docs/commit/6884351229021394417fb6b950b6415e26289796) - jab
* [Troubleshooting guide for OPP hardware](https://github.com/missionpinball/mpf-docs/commit/dc8e949889684f2ce554a142969baad813e2798f) - jab
* [Troubleshooting guide for LISY/APC](https://github.com/missionpinball/mpf-docs/commit/96bd19335df689de0d77751eb40a7f28df2feae6) - jab
* [How to ask questions in the forum for hardware issues](https://github.com/missionpinball/mpf-docs/commit/6e68c0293cea7ec79599e51ad46838205aab7240) - jab
* [Example for transition_out](https://github.com/missionpinball/mpf-docs/commit/e493284001175f083b44ed6e0856830de1f70997) - jab
* [Better widget examples](https://github.com/missionpinball/mpf-docs/pull/313) - public-profile
* [CSSC instructions on Linux](https://github.com/missionpinball/mpf-docs/commit/d3cd70c0c3818a8ee136d2b637c9b0e3f6060daa) - jab (content from Scott Danesi)
* [More OPP troubleshooting](https://github.com/missionpinball/mpf-docs/commit/79075f21d10ab0cc9453aeb657246d65bf86a9fd) - jab
* [Document default_pulse_power/default_hold_power limitations in P3-Roc](https://github.com/missionpinball/mpf-docs/pull/314) - seanirby
* [Troubleshooting for Fadecandy](https://github.com/missionpinball/mpf-docs/commit/ed8fc28b2a644b0925c401e8ae425b32bdbcdf01) - jab
* [Pin2DMD troubleshooting](https://github.com/missionpinball/mpf-docs/commit/a61dcd5b8f2c16b85a4340742ef766c9ea7c0e14) - jab
* Suggest firmware updates for [P/P3-Roc](https://github.com/missionpinball/mpf-docs/commit/9860a1e8b1c5b40973481106d7e38dbb50ab0cbc) and [FAST](https://github.com/missionpinball/mpf-docs/commit/36f273d95e901a08953075bf5bbbd02adbd1b41c) - jab
* [Extend high voltage warning](https://github.com/missionpinball/mpf-docs/commit/01cd9121b24fadb64db8279b87a8180bdd440cbf) - jab
* [Document default recycle times in P/P3-Roc](https://github.com/missionpinball/mpf-docs/commit/5ec5dddd0568d7499d0d375559d1e34d9d511a3d) - jab (content from Gerry)
* [Document debounce and recycle behaviour of autofire_coils](https://github.com/missionpinball/mpf-docs/commit/41830b39151215596dfea4d47e4951a59471c2f4) - jab
* [Document chained lights and numbers vs channels for all platforms](https://github.com/missionpinball/mpf-docs/commit/d82f9446908dd03bdc104560edf999890ae5da55) - jab (see separate blog post)
* [Coil troubleshooting](https://github.com/missionpinball/mpf-docs/commit/089c7e4bd685f0dcb1c85c521ce276c57ae2c333) - jab
* [FAST on Linux troubleshooting](https://github.com/missionpinball/mpf-docs/commit/2279e39b4dca6b22cb7ae9f0858d264c4fac6c7d) - jab
* [Document debounce and recycle behaviour of flippers](https://github.com/missionpinball/mpf-docs/commit/568eff4d6b8c3eb0749166286068c0294e34a095) - jab
* [Notes on RGB and colored inserts](https://github.com/missionpinball/mpf-docs/commit/29468c7171445f8397e4a213a9b19139308950ed) - jab
* [How to install Debian with MPF in VirtualBox](https://github.com/missionpinball/mpf-docs/pull/316) - kylenahas
* [Example for state_machines with placeholders](https://github.com/missionpinball/mpf-docs/commit/7a1277620ed86cd3ccb6b6efebb5334b791bace8) - jab
* [Document start_loop_at/end_loop_at on sounds](https://github.com/missionpinball/mpf-docs/pull/317) - qcapen
* [Document rotation animations](https://github.com/missionpinball/mpf-docs/pull/318) - Coleman
* [Readd tutorial to mpf-examples and test it](https://github.com/missionpinball/mpf-examples/commit/17ea0c323640c0d3de55017cf3c46dbf0c8a2a8b) - jab
* [Fix sound references in demo_man](https://github.com/missionpinball/mpf-examples/pull/13) - kylenahas
* [Add monitor image and config to demo_man](https://github.com/missionpinball/mpf-examples/pull/14) - kylenahas


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

Welcome F4b1-, BENETNATH, public-profile and Compy!

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
