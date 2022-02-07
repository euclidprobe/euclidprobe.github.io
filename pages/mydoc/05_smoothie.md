---
title: "Smoothieware Firmware settings"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: February 5, 2022
permalink: 05_smoothie.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Smoothieware Firmware Settings
---
### Probe device configuration
Smoothieware provides a very good writeup on setting up an NC switch as a Z-probe in its docs. See <a href="smoothiware.org/zprobe" target="blank">smoothiware.org/zprobe</a>

Add the following to the smoothie config file :

```
gamma_min_endstop            nc                 # normally 1.28. Change to nc to prevent conflict, not needed on Azteeg X5

zprobe.enable                true               # set to true to enable a zprobe
zprobe.probe_pin             1.28^             # pin probe is attached to if NO add !
zprobe.slow_feedrate         5                  # mm/sec probe feed rate
#zprobe.debounce_ms          1                  # set if noisy
zprobe.fast_feedrate         100                # move feedrate
zprobe.probe_height          5                  # how much above bed to start probe NB only needed for G32 on delta
zprobe.return_feedrate       0                  # feedrate after a probe, default 0 is double of slow_feedrate (mm/s)
zprobe.max_z                 200                # maximum default travel for the probe command, will use gamma_max if not defined
````

<div style="width:100%;text-align:center;"> 
<a href="images\05_probe-offsets-sm.png" data-lity> <img src="images\05_probe-offsets-sm.png" style="width:450px; border:2px solid CornflowerBlue"></a></div>

