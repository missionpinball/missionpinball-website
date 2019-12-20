---
layout: post
author: jab
title: Tested examples in the MPF documentation
tags: [MPF]
---
We have been testing the examples in our documentation for a while but we never
showed you which bits are tested and how.
This has changed and you can now see the tests inside the docs.

Have a look at this
[example doc page with tests](http://docs.missionpinball.org/en/dev/game_logic/scoring/index.html).
Below the first example you find "This example is tested to be valid MPF
config. However, it is not integration tested."
This basically means that we will tested that MPF started with that config
without raising any errors on startup.
You can rely that this config is valid yaml and does not contain invalid
settings or values.
However, the game might still crash when you press the start button for
some logic or runtime issues.

If you looks at the second snippet you will find "This example is tested to be
valid MPF config. Additionally, our integration test passed. Click to show the
test and full config."
This means that not only does MPF start but we also executed some kind of test.
If you click on the text will see the full config with tests.
Sometimes we hide non-relevant stuff such as switch/coil definitions in
examples to keep it simple.
In this case you will find this test:

    ##! test
    start_game
    assert_player_variable 0 multiplier
    start_mode my_mode
    assert_player_variable 1 multiplier
    post score_something
    assert_player_variable 100 score
    post increment_multiplier
    assert_player_variable 2 multiplier
    post score_something
    assert_player_variable 300 score

First it will start a (single player) game and check that the multiplier
variable is zero.
Afterwards, it starts "my_mode", checks that the multiplier is now one and 
triggers some scoring.
After verifying scoring it increases the multiplier and verifies that it is
respected during scoring.

If you want to run the test youself you can copy the snippet to a file and
run it locally using "mpf test your_file.txt".
You can also use that to create your own small tested snippets.

The test above only covers MPF and not MPF-MC.
In case there are any slides or widgets they are mostly untested (except for
valid syntax). 
There are also some [snippets](http://docs.missionpinball.org/en/dev/game_logic/shots/integrate_shots_with_shows_lights_sounds_widgets_or_slides.html)
which require MPF-MC.
This example also contains a test which asserts that the correct widgets show
at the right time.
We do not test MPF-MC on all of the examples because those tests are two
magnitudes slower than pure MPF tests and most snippets do not contain
any slides or widgets anyway.

[Contributions to the docs](http://docs.missionpinball.org/en/dev/about/contributing_to_mpf_docs.html)
are welcome.
Even more if they contain tested snippets.
We run those tests regularly to make sure that we do not break any real
world examples. 
