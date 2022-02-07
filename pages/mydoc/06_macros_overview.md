---
title: "Euclid Probe Deploy & Retract Strategies"
keywords: probe dock, tool mount
tags: [FAQ]
permalink: 06_macros_overview.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Deploy & Retract Strategies
---
### Overview
The overall concept to deploying and retracting Euclid Probe is to approach the probe dock from the side, move over the probe so that the magnetic force between magnets lifts the probe up from the well, pauses for the firmware to recognize that the probe state has changed, then exit the dock.  

When the magnets have picked up the probe, the probe should be aligned with the exit gate so the probe can travel out of the dock.

To retract or dock the probe, the process is reversed: approach and then enter the dock, park the carriage over the dock well, move quickly to the side, swiping the magnets apart. When the magnets are swiped apart, the probe will drop into the well, below the level of the exit gate and be secure.

Care must be taken to consider the order of operations in the overall homing and bed leveling scheme. It is recommended that a different macro be written to deeply and retract the probe, and to call them when homing, probing or bed leveling.

<div style="width:100%;text-align:center;">
  <a href="images\06-probe_deploy-1024x610.jpg" data-lity>
    <img src="images\06-probe_deploy-1024x610.jpg" style="width:300px; border:2px solid CornflowerBlue">  </a>
    <p>Click image to enlarge</p>  
</div>  


