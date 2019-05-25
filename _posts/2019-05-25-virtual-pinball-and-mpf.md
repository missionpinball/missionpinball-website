---
layout: post
author: mfuegemann
title: Running your MPF game on a VPX Virtual Pinball Table
tags: [Rust, Spike, MPF]
---
After some months the MPF-VPX bridge proof of concept has been brought to live for real.
We were able to successfully link MPF and VPX so that the VPX table is emulating the hardware for a MPF machine.
After the first successful switch hits and lamp states have been sent, the functionality of the bridge has been extended.
At the moment, lights, switches and solenoids are handled to fully.
Mechs and Magnets are still missing but will be worked on in the future.

The bridge will connect to the running MPF machine when you start your VPX
table.
As the VPX table is used only to emulate the hardware and should not contain
any game logic.

At the moment the latest VPX platform is contained in MPF 0.53 dev (see: [Installing dev version](http://docs.missionpinball.org/en/dev/install/windows.html#install-mpf)).
This version is currently necessary for the [bridge](https://github.com/missionpinball/mpf-vpcom-bridge) to work.
However, this will very likely make it into the upcoming 0.53 stable release.
You can also read our [Documentation about the VPX platform](http://docs.missionpinball.org/en/dev/hardware/virtual/virtual_pinball_vpx.html).

## Installation

Copy the file `register_vpcom.py` to your local machine.
To register the bridge run a CMD shell as Administrator, then

```
python register_vpcom.py --register
``` 

(You can use ```--unregister``` to uninstall the bridge)

## Use VPX in MPF

In your ```config.yaml``` configure virtual_pinball as your platform: 

```
hardware: 
    platform: virtual_pinball
```

or if you already have physical hardware configured start MPF with the ```--vpx``` commandline option (similar to ```-X```):

```
mpf both --vpx
```


## What to do in VPX

In VPX you need to adjust your script to talk to MPF.
You can also looks this up in the example project inside the [bridge repository](https://github.com/missionpinball/mpf-vpcom-bridge).
The GameName set in VPX is not used to check or validate the MPF machine.

### Setup controller and timers

- add ```Set Controller = CreateObject("MPF.Controller")```
- add a Timer ```MPFTimer``` with an interval of 10 to 50ms. Keep this well below the minimal ```default_pulse_ms``` set in MPF for solenoids
- add a ```Sub MPFTimer_Timer``` to update all the lights and solenoids

### In Table_Init
 
- call Controller.run
- set the Trough switch(es) or create balls for a physical Trough (as in the demo table)
- init NC switches to False

### In Drain_Hit (for 1-Ball games)
- set the Trough switch(es) 

### To use autofire_coils (Slings, Pops etc)
- add a droppable wall to each bumper. This will be used in ```Sub CheckAutofireCoils``` to disable/enable the bumper
- if necessary place an invisible wall behind the slingshots to stop the ball once the slingshots are disabled
- add each autofire object in VPX to ```Sub CheckAutofireCoils```
- use the normal ```Slingshot_Slingshot``` and ```Bumper_Hit``` events

### Switch Handling
- add ```Controller.Switch(MPFSwitchNumber)=SwitchState``` to the ```Switch_Hit/_Unhit``` events. Use "" to include string type numbers
- add ```Controller.PulseSW(MPFSwitchNumber)``` to the ```Switch_Hit``` event of targets, slingshots and bumpers

### Controlled Lights (all types)
- create a collection "ControlledLamps"
- assign all controlled VPX lamps (Matrix, GI, LED, Flashers) to the collection "ControlledLamps" and call ```InitLamps```

### LEDs and Lamps
- in ```Sub UpdateLamps``` add a case for every MPF light and LED number, setting the state of the VPX lamp/LED. Use "" to include string type numbers

### GI strings 
- create a collection for each GI string, assign the GI lamps to the collections as needed
- assign all GI lamps to the collection "ControlledLamps" and call``` InitLamps```
- in ```Sub UpdateGI``` add a case for every MPF gi string number, setting the state of the VPX GI collection. Use "" to include string type numbers

### Flashers
- assign all flasher lamps to the collection "ControlledLamps" and call ```InitLamps```
- in ```Sub UpdateFlashers``` add a case for every MPF flasher number, setting the state of the VPX flasher. Use "" to include string type numbers

### Solenoids
- add all normal solenoids to the ```Sub InitSolenoids```, to initialize them als ```False```
- in ```Sub UpdateSolenoids``` add a case for every MPF coil number, setting the state of the VPX solenoid. Use "" to include string type numbers

### Flippers
- add the Flipper routines (```Solenoids``` and ```KeyUp/KeyDown```) as in the demo table. Flippers are handled as autofire coils and can be enabled/disabled using hrdware rules.

## To run a game
1. start VPX as Administrator
2. start MPF, wait until the display has been initialized
3. start VPX table

To exit a game shut down the VPX table first

Any problems getting VPX and MPF to work?
Let us know in the [MPF-Users forum](https://groups.google.com/forum/#!forum/mpf-users)!
