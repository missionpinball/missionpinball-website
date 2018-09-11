---
layout: post
author: jab
---
What happened in MPF-land in August 2018?
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

# Current release 0.50

We released 0.50.13 with bugfixes.

## Changes

None

## Bugfixes

* [Restore Diverter State After Ball Search](https://github.com/missionpinball/mpf/commit/7930fbc4691676edb87d5601245dd460e18562f0)

# Dev release (future 0.51)

We pushed dev-7.

## Changes

* [Improve performance without logging](https://github.com/missionpinball/mpf/commit/b870147b3031f4ab5cea90911269013b8d86f3ac)

## Bugfixes

* [Fix debug flag in P-Roc and P3-Roc](https://github.com/missionpinball/mpf/commit/015fc4d8508ffadf9324100a5d9280dd4e781b49)
