---
layout: post
author: jab
title: Emulating Segment Displays in MPF-MC using a Glow Effect Shader
tags: [GLSL, MPF-MC, segment displays]
---
Do you want realistically looking segment displays on an LCD using MPF-MC?
Then this post is for you!

Sean has been working recently on emulating a segment display for his game.
It needed a glowing type of shader effect in order to achieve a convincing
result so he decided to add one to his local copy of MPF-MC.
As it turned out really great and it looked really awesome he posted 
a [Pull Request](https://github.com/missionpinball/mpf-mc/pull/400)
others might use it as well.
This PR contains a general effect, so if you who want to emulate a segment
display as he did you also have to set up the fonts and such using widgets in
your game.
He also added
[documentation](https://github.com/missionpinball/mpf-docs/pull/308) for the
shader.

Without the effect:
<iframe src="https://giphy.com/embed/TgJ9FcKc7dA2SxPLft" width="480" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/TgJ9FcKc7dA2SxPLft">via GIPHY</a></p>

With the effect:
<iframe src="https://giphy.com/embed/JQjAQl0nlC3wK70imW" width="480" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/JQjAQl0nlC3wK70imW">via GIPHY</a></p>


Thank for your Sean for this great addition!
In the future we hope to turn this into a very easy to use
"virtual segment display" similar to virtual DMDs in MPF-MC. 

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
