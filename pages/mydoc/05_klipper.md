---
title: "klipper Firmware settings"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: February 5, 2022
permalink: 05_klipper.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: klipper Firmware Settings
---
### Probe device configuration
Configuring Euclid Probe in klipper is similar to defining and endstop switch. The following is an example of the probe section in the printer configuration file.


For more reference information see <a href="https://www.klipper3d.org/G-Codes.html?h=probe#probe" target="blank"> klipper Command reference</a>

<div style="width:100%;text-align:center;"> 
<a href="images\05_probe-offsets-sm.png" data-lity> <img src="images\05_probe-offsets-sm.png" style="width:450px; border:2px solid CornflowerBlue"></a></div>

This is an example of the relevant printer.cfg entries:  

```
[force_move]
#enable_force_move: False
#   Set to true to enable FORCE_MOVE and SET_KINEMATIC_POSITION
#   extended G-Code commands. The default is false.
```  

```
[respond]
#default_type: echo
#   Sets the default prefix of the "M118" and "RESPOND" output to one
#   of the following:
#       echo: "echo: " (This is the default)
#       command: "// "
#       error: "!! "
#default_prefix: echo:
#   Directly sets the default prefix. If present, this value will
#   override the "default_type".
```   


```
[probe]
##    Euclid Probe
pin: ^P1.24 # ZMax on SKR 1.1
x_offset: -20
y_offset: -2.0
z_offset: 12.0
speed: 5
samples: 2
samples_result: average
sample_retract_dist: 5.0
samples_tolerance: 0.050
samples_tolerance_retries: 3
lift_speed: 30

[include euclid.cfg]
# where euclid.cfg is the filename with all the probe deploy adn retract and probing macros

```  

### Setting Z offset elevation
See klipper configuration reference section on <a href="https://www.klipper3d.org/G-Codes.html?h=probe#probe_calibrate" target="blank">PROBE_CALIBRATE</a> for the klipper procedure on setting the Z probe offset. 