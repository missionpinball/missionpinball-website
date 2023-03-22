---
layout: post
author: jab and markinc
title: The Awesome But Little Known Lightshow Creator For MPF
tags: [lightshow, MPF]
---
MPF supports playing light shows out of files in your config folder.
Those are human readable and can be created by hand.
But isn't that a bit cumbersome for larger shows?
Especially, if you want to swipe over all (or most) of your LEDs this might
take days.
Luckily, there is a tool for that.

[Shows](https://docs.missionpinball.org/en/dev/shows/index.html) in MPF are
written in YAML and can be used
[universally](https://docs.missionpinball.org/en/dev/config_players/index.html)
to control all kinds of things (such as
[lights](https://docs.missionpinball.org/en/dev/config_players/coil_player.html),
[coils](https://docs.missionpinball.org/en/dev/config_players/coil_player.html),
[slides](https://docs.missionpinball.org/en/dev/config_players/slide_player.html),
[widgets](https://docs.missionpinball.org/en/dev/config_players/widget_player.html),
[sounds](https://docs.missionpinball.org/en/dev/config_players/sound_player.html)
and [more](https://docs.missionpinball.org/en/dev/config_players/index.html)).
Basically, shows are a list of actions combined with a duration after which
the next element in the list is played.
Here is an example of a light show with three lights which sequentially turn
blue over one second:

    #show_version=5
    - duration: .25
      lights:
        l_arrow_1: off
        l_arrow_2: off
        l_arrow_3: off
    - duration: .25
      lights:
        l_arrow_1: blue
        l_arrow_2: off
        l_arrow_3: off
    - duration: .25
      lights:
        l_arrow_1: blue
        l_arrow_2: blue
        l_arrow_3: off
    - duration: .25
      lights:
        l_arrow_1: blue
        l_arrow_2: blue
        l_arrow_3: blue

In this simple example it totally makes sense to create the show by hand.
You could also throw in
[tokens](https://docs.missionpinball.org/en/dev/shows/tokens.html)
for the lights and reuse the show all
over the machine for different light triples.

However, imagine you want to swipe over all lights in your machine.
That would be a lot of text and also hard to get right manually.
Luckily, Mark, the maker of the
[Nightmare before Christmas custom pinball machine](https://pinside.com/pinball/forum/topic/the-nightmare-before-christmas),
created the awesome
[MPF Lightshow Creator](https://docs.missionpinball.org/en/dev/tools/showcreator/index.html).

![MPF Lightshow Creator](https://docs.missionpinball.org/en/dev/_images/showcreator.png)

The tool allows you to animate shapes (i.e. a star in the example) across your playfield lights.

You might ask: How does it know where my lights are located on the playfield?

Luckily, you probably already have them set if you used the MPF Monitor:

![MPF Monitor](https://docs.missionpinball.org/en/dev/_images/mpf-monitor.jpg)

It allows you to use drag and drop to position all your switches and lights on
a playfield image.
Those positions are then saved to the ``monitor/monitor.yaml`` file in your
machine folder.

All you have to do is point the light show creator to the ``monitor/monitor.yaml`` file on startup.

You set the start and end positions, rotations, scales and colors of that shape
anywhere you want over the playfield.

Here we start with a gradient bar at the top of the playfield in a pink color.
![MPF Lightshow Creator](https://docs.missionpinball.org/en/dev/_images/showcreator_start.png)

We want the final position to be here at the bottom, in a darker red shade.
![MPF Lightshow Creator](https://docs.missionpinball.org/en/dev/_images/showcreator_end.png)

You can then adjust the length of the animation in milliseconds and hence the number of steps in the final show.
In this example, the shape will be moved from the start to finish in 24 steps.

Based on these settings, it will create a light show for you which contains all needed commands
per step for each of the lights the shape passes over. Lightshow playback speed can be adjusted in MPF.

You're not restricted to just the included shapes.  You can make your own shapes and drop them in the shapes folder.
![MPF Lightshow Creator](https://docs.missionpinball.org/en/dev/_images/showcreator_shapes.png)

Once you get the hang of animating a single shape, you can go further by adding in more shapes.
You can add a total of 256 shapes in animation segments.
Each segment can be set to ``concurrent`` (start and end same time as the previous segment)
or ``follow`` (start after previous segment)
This allows for more interesting multipart shows. For example you could have several color swipes coming from different directions
one after the other or effects like multiple spotlights moving across the playfield like a hollywood premiere.

The tool is still evolving and will probably gain more features over time.
It is handy for rendering static shows which will not change during runtime.
If you want to render shows dynamically (using your GPU) you can also use
[your lights as display in MC](https://docs.missionpinball.org/en/dev/config_players/display_light_player.html)
but that will cost you much more in resources during runtime than offline generated shows.

You can reach us in the [MPF-Users forum](https://groups.google.com/forum/#!forum/mpf-users).
Questions, discussion and feedback are very welcome!