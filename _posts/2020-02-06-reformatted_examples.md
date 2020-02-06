---
layout: post
author: jab
title: Reformatted examples in docs for a better copy and paste experience
tags: [hardware, MPF, pin2dmd]
---
We reformatted all our examples to use consistent spaces to reduce errors
because of copy and paste from examples.

Unfortunately, YAML formatting has caused some headaches amount our users.
Just to give you an idea how a new user feels when copy and pasting examples
from our docs with varying indent watch
[deadflip finding out about spaces](https://www.twitch.tv/deadflip/clip/FragileHardCheddarCoolCat).
This will hopefully not happen anymore as we changed all example to a
consistent with two spaces per level and also test all our examples regularly
in our CI/CD chain which builds the docs.
You can have a look at the [changeset](https://github.com/missionpinball/mpf-docs/pull/274)
which changed 289 files in the docs.

How did you do this?
As there are currently 783 tested examples in the docs we did not reformat
everything by hand.
Instead we create a new [command](https://github.com/missionpinball/mpf/pull/1499)
`mpf format <file>` to reformat an example, docs file or config file.
You can use it to your config if you like:

```
$ mpf format config/switches.yaml 
Parsing single test config/switches.yaml.
Config is not linted.
--- 
+++ 
@@ -416,9 +416,9 @@
 
 keyboard:
   o:
-    event:  debug_front_to_back
+    event: debug_front_to_back
   p:
-    event:  debug_back_to_front
+    event: debug_back_to_front
   y:
     switch: s_test_flip_left
   x:

Not writing back changes. Use --yes to do this. 
```

It will first show you what it you change but does only apply changes if you
pass `--yes` to the end of the commandline.
We recommand you to put your machine configs into a git repository.
In case `mpf format` accidentally breaks something you can simply revert the
file.
Please let us know if you find any cases where it fails to parse or format your
config.

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
