---
layout: post
author: jab
title: "New Supported Hardware: PIN2DMD - A Color LED Dotmatrix Controller for Virtual and Real Pinballs"
tags: [hardware, MPF, pin2dmd]
---
In MPF 0.54-dev, we added support for PIN2DMD.
PIN2DMD is a RGB DMD display which connects to a PC via USB.
It exists in a 128x32 (traditional pinball) and 192x64 pixel (large SEGA/Data
East displays) version.
Those can now be used in your custom game with MPF!

To use PIN2DMD in MPF you should first install your panel as described on the
[PIN2DMD homepage](https://pin2dmd.com/) (steps hardware and firmware).
Afterwards, configure your machine as follows:

1. Add `pin2dmd` to your hardware section:

    ```yaml
    hardware:
      rgb_dmd: pin2dmd
    ```

2. Configure a display for your DMD:


    ```yaml
    displays:
      window:  # on screen window - useful for debugging without real hardware
        width: 600
        height: 200
      dmd:  # source display for the DMD
        width: 128      # 192 if you got a 192x64 pin2dmd panel
        height: 32      # 64 if you got a 192x64 pin2dmd panel
        default: true

    rgb_dmds:
      default:  # your DMD
         brightness: .2     # adjust the brightness of your display if it is too bright
         fps: 30
    ```

3. Configure your pin2dmd hardware:

    ```yaml
    pin2dmd:
        # debug: True           # uncomment this if you experience any issues and need debug output
        resolution: 128x32      # or 192x64 depending on your panel
        panel: rgb              # or rbg if colors are swapped
    ```

This is how a 128x32 pixel PIN2DMD looks in action:

![128x32 pixel PIN2DMD with MPF](https://pin2dmd.com/wp-content/uploads/2020/01/mpf-test.jpg "128x32 pixel PIN2DMD with MPF")

And this is how a 192x64 pixel PIN2DMD looks:

![192x64 pixel PIN2DMD with MPF](https://pin2dmd.com/wp-content/uploads/2020/01/mpf192x64.jpg "192x64 pixel PIN2DMD with MPF")

For more details follow our
[tutorial on RGB DMDs in MPF](https://docs.missionpinball.org/en/dev/displays/display/rgb_dmd.html)
or the [tutorial for PIN2DMD in MPF](https://docs.missionpinball.org/en/dev/hardware/pin2dmd/index.html)
in the MPF docs.

Thanks to Lucky1 for providing sample code, testing with real hardware and taking pictures!

Did we forget anything? Please let us know!
Discussions in [MPF-Users](https://groups.google.com/forum/#!forum/mpf-users).
