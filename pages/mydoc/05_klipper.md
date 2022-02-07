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

This is an example of the relevant printer.cfg entry:  


```
; [probe]
##    Euclid Probe
pin: ^PA0 # pin number PA0, enable the hardware pull-up resistor 
x_offset: -16.48
y_offset: -29.35
z_offset: 0.91
speed: 5
samples: 2
samples_result: average
sample_retract_dist: 3.0
samples_tolerance: 0.0075
samples_tolerance_retries: 3
```  

### Setting Z offset elevation
See klipper configuration reference section on <a href="https://www.klipper3d.org/G-Codes.html?h=probe#probe_calibrate" target="blank">PROBE_CALIBRATE</a> for the klipper procedure on setting the Z probe offset. 