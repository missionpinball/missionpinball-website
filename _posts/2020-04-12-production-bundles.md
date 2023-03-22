---
layout: post
author: jab
title: Production Config Bundles for Fast Startup on Production Hardware
tags: [software, MPF, production]
---
How we make the start of your production machine fast and smooth?

YAML is quite slow to parse and reading configs dominates the startup time
of MPF and MPF-MC.
This is mostly fine during development and we can partially mitigate the costs
by caching.
However, things are different when running a production machine as caching
will not work on a cold boot with a typical read-only setup.
Usually production machine setups use less beefy computers with slower disks
which makes thinks even worse.

To get out of this we added an production flag to MPF 0.54 which will use
pre-compiled config bundles for much faster start-up times.
Additionally, this will disable some expensive config and runtime validations
to increase performance.
Furthermore this will reduce the amount of debug output.

How does it work?
First run ``mpf build production_bundle`` which will create
``mpf_config.bundle`` and ``mpf_mc_config.bundle``.
You have to recreate those files after every config, mode or show change.
Those bundles include all yaml files but not any other assets (such as
videos or sounds).
Second, add the ``-P`` flag to the commandline to run MPF in production mode.

Find out more about it in the
[MPF docs about Tuning Software for Production](https://docs.missionpinball.org/en/dev/finalization/software.html#run-mpf-in-production-mode).

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
