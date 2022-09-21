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
## General klipper firmware setup
We have broken the klipper setup into two parts- the general hardware configuration in the ```printer.cfg``` to be consistent with all hardware definitions and a pointer in the ```printer.cfg``` to include the ```euclid.cfg``` file for the macros. Please look at both parts. 

### Probe device configuration
Configuring Euclid Probe in klipper is similar to defining and endstop switch. The following is an example of the probe section in the printer configuration file.

For more reference information see <a href="https://www.klipper3d.org/G-Codes.html?h=probe#probe" target="blank"> klipper Command reference</a>

<div style="width:100%;text-align:center;"> 
<a href="images\05_probe-offsets-sm.png" data-lity> <img src="images\05_probe-offsets-sm.png" style="width:450px; border:2px solid CornflowerBlue"></a></div>
<br>
<hr>

Below is an example of the relevant printer.cfg entries. Euclid macros make use of ```force_move``` and ```respond```. 

Macros for probe deploy and stow are covered <a href="https://euclidprobe.github.io/06_klipper3.html">here</a>.   

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
# where euclid.cfg is the filename with all the probe deploy and retract and probing macros

```  
Here are the examples of euclid configuration files. <a href="https://github.com/nionio6915/Euclid_Probe/tree/main/Firmware_Examples/Klipper" target="blank">euclid.cfg </a> files. 

Simple Version: 00-euclid_exampleV3.cfg is a generic template with hard coded position variables and simple macros. 

Version with more features: 00-euclid_exampleV5.cfg and uses array variables and more fully featured macros. It takes a bit more work to set up. Pay attention to the ```## @TODO``` statements where user input is required. This version is contributed by yolodubstep, and is a stripped down version of his configs. Yolodubstep's most current configs are here- <a href="https://github.com/blalor/vcore3-ratos-config" target="blank">Yolodubstep V-Core files.</a>. 

The best documented and most comprehensive set of klipper configuration files are from <a href="https://github.com/rkolbi/voron2.4" target="blank">deepsiks </a>  
VORON 2.4 / 350mm/ 24v / BTT Octopus / Bondtech LGX / Phaetus Dragon HF /Bondtech .4 CHT / Euclid Probe /Hall Effect Endstops  

The other various printer configurations are in the user submitted klipper folder <a href="https://github.com/nionio6915/Euclid_Probe/tree/main/Firmware_Examples/Klipper/user_contrib" target="blank"> in the Firmware Examples/klipper folder</a>.  


### Setting Z offset elevation
See klipper configuration reference section on <a href="https://www.klipper3d.org/G-Codes.html?h=probe#probe_calibrate" target="blank">PROBE_CALIBRATE</a> for the klipper procedure on setting the Z probe offset. 