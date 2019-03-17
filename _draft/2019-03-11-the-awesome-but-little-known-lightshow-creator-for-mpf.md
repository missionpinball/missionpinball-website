---
layout: post
author: jab
title: The Awesome But Little Known Lightshow Creator For MPF
tags: [lightshow, MPF]
---
MPF supports playing light shows out of files in your config folder.
Those are human readable and can be created by hand.
But isn't that a bit cumbersome for larger shows?
Especially, if you want to swipe over all (or most) of your LEDs this might
take days.
Luckily, there is a tool for that.

[Shows](http://docs.missionpinball.org/en/dev/shows/index.html) in MPF are
written in YAML and can be used
[universally](http://docs.missionpinball.org/en/dev/config_players/index.html)
to control all kinds of things (such as
[lights](http://docs.missionpinball.org/en/dev/config_players/coil_player.html),
[coils](http://docs.missionpinball.org/en/dev/config_players/coil_player.html),
[slides](http://docs.missionpinball.org/en/dev/config_players/slide_player.html),
[widgets](http://docs.missionpinball.org/en/dev/config_players/widget_player.html),
[sounds](http://docs.missionpinball.org/en/dev/config_players/sound_player.html)
and [more](http://docs.missionpinball.org/en/dev/config_players/index.html)).
Basically, shows are a list of actions combined with a duration after which
the next element in the list is played.
Here is an example of a light show with three light which sequentially turn
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
[tokens](http://docs.missionpinball.org/en/dev/shows/tokens.html)
for the lights and reuse the show all
over the machine for different light triples.

However, imagine you want to swipe over all lights in your machine.
That would be a lot of text and also hard to get right manually.
Luckily, Mark, the maker of the
[Nightmare before Christmas custom pinball machine](https://pinside.com/pinball/forum/topic/the-nightmare-before-christmas),
created a the awesome
[MPF Lightshow generator](http://docs.missionpinball.org/en/dev/tools/showcreator/index.html).

![MPF Lightshow Creator](http://docs.missionpinball.org/en/dev/_images/showcreator.png)

The tool allows you to set a shape (i.e. a star in the example), choose a start
and an end position and color.
Based on that it will create a light show for you which contains one section
per step (at a defined frame rate). 
Neat right?
You might ask: How does it know where my lights are located on the playfield?

Luckily, you probably already have them set if you used the MPF Monitor: 

![MPF Monitor](http://docs.missionpinball.org/en/dev/_images/mpf-monitor.jpg)

It allows you to use drag an drop to position all your switches and lights on
a playfield image.
Those positions are then saved to the ``monitor/monitor.yaml`` file in your
machine folder.
All you have to do is to copy the lights to the ``ledsloc.txt`` file in the
show creator and your are good to go (this might become unnecessary in the
future).

The tool is still evolving and will probably gain more features over time.
It is good to render static shows which will not change during runtime.
If you want to render shows dynamically (using your GPU) you can also use
[your lights as display in MC](http://docs.missionpinball.org/en/dev/config_players/display_light_player.html)
but that will cost much more resources during runtime than offline generated
shows.


Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
