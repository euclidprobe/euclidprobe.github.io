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
## Probe Deployment Overview
The overall concept to deploying and retracting Euclid Probe is to approach the probe dock from the side, move over the probe so that the magnetic force between magnets lifts the probe up from the well, pauses for the firmware to recognize that the probe state has changed, then exit the dock.  

Care must be taken to consider the order of operations in the overall homing and bed leveling scheme. It is recommended that a different macro be written to deeply and retract the probe, and to call them when homing, probing or bed leveling.


This graphic is used to illustrate the positions and movements in various firmware examples.  The dock is located in the bottom left hand corner of the picture (X0 Y0) and dock orientated vertically, so that the probe exits in the +Y direction.     

<div style="width:100%;text-align:center;">
  <a href="images\06_DeploySteps.png" data-lity>
    <img src="images\06_DeploySteps.png" style="width:300px; border:2px solid CornflowerBlue">  </a>
    <p>Click image to enlarge</p>  
</div>  

When the magnets have picked up the probe, the probe should be aligned with the exit gate so the probe can travel out of the dock.

<div style="width:100%;text-align:center;">
  <a href="images\02_Dock_Height_2.jpg" data-lity>
    <img src="images\02_Dock_Height_2.jpg" style="width:300px; border:2px solid CornflowerBlue">  </a>
    <p>Click image to enlarge</p>  
</div>  

## Probe Retraction Overview 
To retract or dock the probe, the process is reversed: approach and then enter the dock, park the carriage over the dock well, move quickly to the side, swiping the magnets apart. When the magnets are swiped apart, the probe will drop into the well, below the level of the exit gate and be secure.


<div style="width:100%;text-align:center;">
  <a href="images\06_Retract Steps.png" data-lity>
    <img src="images\06_Retract Steps.png" style="width:300px; border:2px solid CornflowerBlue">  </a>
    <p>Click image to enlarge</p>  
</div>  


