---
layout: post
author: jab
title: Twitch Integration in MPF
tags: [MPF, Twitch]
---
Want to stream your custom pinball machine on Twitch?
Thanks to Mark Seiden your machine can now react to commands and messages
from your Twitch chat.

Mark developed this feature back in 2018 and used it on
[his twitch channel](https://twitchtracker.com/thearrrrrcade) since then.
Recently, he [upstreamed it as a MPF plugin](https://github.com/missionpinball/mpf/pull/1530)
to allow others to use it as well.
We heard that there is a lot of excitement about the feature and 
expect additional features to be added in the near future.

If you want to know more have a look at the
[documentation about twitch_cient](https://docs.missionpinball.org/en/dev/config/twitch_client.html).
The plugin will set [twitch_* machine variables](https://docs.missionpinball.org/en/dev/machine_vars/index.html)
which can be used in slides/widgets and more.
Additionally, it posts [twitch_* events](https://docs.missionpinball.org/en/dev/events/index.html)
which can be used to trigger sounds, widgets or logic. 

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
