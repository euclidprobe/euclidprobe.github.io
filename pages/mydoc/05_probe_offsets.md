---
title: "Probe Offsets"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: October 13, 2022
permalink: 05_probe_offsets.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Probe Offset Settings
---

### Locating Probe Offsets
The probe offset position relative to the nozzle is needed in all firmware configurations. The following image shows the probe location that used in some of the following firmware examples.  

<div style="width:100%;text-align:center;"> <a href="images\05_probe-offsets.png" data-lity> <img src="images\05_probe-offsets.png" style="width:450px; border:2px solid CornflowerBlue"></a></div>

While having a CAD model is nice to reference, its not a requirement. A simple ruler, held on edge can be used to measure the centerline distances between the magnets and the nozzle.  
<div style="width:100%;text-align:center;"> <a href="images\04-wiring\pcb_parts\Slide1.PNG" data-lity> <img src="images\04-wiring\pcb_parts\Slide1.PNG" style="width:450px; border:2px solid CornflowerBlue"></a></div>  


Another good resource for determining the probe offsets is discussed on this <a href="https://duet3d.dozuki.com/Wiki/Test_and_calibrate_the_Z_probe#Section_Here_is_an_easy_way_to_measure_the_offset" target="blank">Duet dozuki page.</a>  

{% include tip.html content="Configure the Z probe offset at the temperatures that you will most be printing at: nozzle, bed and chamber. The offset will vary if you calibrate at 180C nozzle, 50C bed and 20C chamber/ambient compared to 245C nozzle, 100C bed and 60 chamber!" %}


### Probe Z Offset
To calibrate the Z probe trigger height, verify that probe probe stops when it senses the bed. 
  1. Cancel any currently active mesh compensation. 
      * RRF use gcode ```M561``` 
      * klipper use ```BED_MESH_CLEAR```
  2. Deploy the probe (eg M401) and use the X and Y jog buttons to position the nozzle over the center of the bed. 
  3. Jog the nozzle down until it is just touching the bed or just gripping a feeler gauge of known thickness or a sheet of paper. A Pokemon card is reported to be 0.2mm in thickness. If the firmware doesn't let you jog it down far enough, send M564 S0 to disable axis limits.
  4. Once you have the nozzle touching the bed or feeler gauge, send command ```G92``` to tell the firmware that the head is at that position. 
      * G92 Z=0 if it just touching the bed
      * G92 Z=0.2 if using a 0.2mm feeler gauge
      * G92 Z=0.1 if using a piece of copy paper
  5. Jog the head up by 15 to 20mm
  6. Probe the bed
      * RRF use ```G30 S-1``` 
      * Marlin use ```G30``
      * klipper use ```PROBE``` 
     The nozzle will descend or the bed rise until the probe triggers and the Z height at which the probe stopped will be reported. You will likely need to manaully move the bed to break contact with the probe. 
     ```G0 Z15```
  7. Repeat from steps 5 two or three times to make sure that the trigger height is consistent.

The reported height is the Z probe height to use in your firmware.

RRF: refer to https://docs.duet3d.com/en/User_manual/Connecting_hardware/Z_probe_testing
klipper: refer to https://www.klipper3d.org/Probe_Calibrate.html

