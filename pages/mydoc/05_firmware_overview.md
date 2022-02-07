---
title: "Firmware Setting Overview"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: February 5, 2022
permalink: 05_firmware_overview.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Firmware Setting Overview
---

### Locating Probe Offsets
The probe offset position relative to the nozzle is needed in all firmware configurations. The following image showing the probe location is used in the following firmware examples.

Another good resource for determining the probe offsets is discussed on this <a href="https://duet3d.dozuki.com/Wiki/Test_and_calibrate_the_Z_probe#Section_Here_is_an_easy_way_to_measure_the_offset" target="blank">Duet dozuki page.</a>

<div style="width:100%;text-align:center;"> <a href="images\05_probe-offsets.png" data-lity> <img src="images\05_probe-offsets.png" style="width:450px; border:2px solid CornflowerBlue"></a></div>

### Probing Speeds
In general terms, we recommend singe probing speeds of 2mm/sec to start with.  
If your firmware can perform 2-speed probing, 5mm/sec & 2mm/sec would be reasonable starting points.  

We recommend that users perform their own repeatability tests to fine tune the speeds if faster speeds are desired. 

Here is the previous example of a single switch’s probing results performed at room temperature. Note the trends of the blue vertical bars showing the trigger point in the speed ranges noted at the top.   

Also not the population of the probe points in relationship to the standard of deviation bars noted in orange. The standard of deviation bars are for the total population.

<div style="width:100%;text-align:center;">
  <a href="images\00-ProbeTest57_19_45-768x559.png" data-lity>
    <img src="images\00-ProbeTest57_19_45-768x559.png" style="width:300px; border:2px solid CornflowerBlue">
  </a>
  <p><span style="color:blue">Click image to enlarge</span>.</p>
  
</div>
