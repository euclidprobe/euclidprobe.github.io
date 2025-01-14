---
title: "Euclid Probe Deployment Planning"
keywords: assembly planning
tags: [assembly, planning]
last_updated: January 29, 2022
permalink: 01_preflight.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Euclid Probe Deployment Planning 
---

###  What voltage?  
Most controllers use either 3.3V or 5V for their MCU, aka <b>VCC</b>. Most of the modern controllers are also VCC voltage tolerant on their IO pins- meaning they probably wont get hurt if you accidentally feed a pin VCC voltage.  The most reliable, least risky connection of Euclid PRobe to your controller is via an unused endstop pin.  

We have developed a 24V version of Euclid probe for direct wiring on 24V toolhead boards and dedicated 24V capable probe ports. However, using the higher voltage comes with more risk- the controller logic is still 3.3V/5V and if you are not careful, or have a happy accident and put 24V on an input pin, you will create the blue magic smoke. 

{% include tip.html content="After soldering, clip the protruding solder pins flush and cover the exposed solder joints with a bit of tape or paint with nail polish to insulate. This keeps the blue magic smoke in the genie bottle!" %}


###  Determine the best orientation of the tool board and probe before assembly.  
The orientation of the tool board does not necessarily have to match the orientation of the probe. 

The probe is designed to enter the dock like an arrow, the wider section self-centering the PCB in case of misalignment. 

The 'arrows' can point in opposite ways. In fact, this is the orientation for an i3 style printer like an Ender3 or Wanhao i3, where the mount points to Xmin and the probe enters the moving dock towards Xmax.   

Guide blocks used to aid in the assembly and for hole drilling and tap aligning are <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/stls/Assembly%20Jigs' target="_blank"> here.</a> They are not required but helpful to users who are not confident in their assembly skills. 

<a href='https://github.com/nionio6915/Euclid_Probe/raw/main/stls/Assembly%20Jigs/soldering_jigV5-0.2mm_margin.stl'>Solder and Drilling Jig with 0.2mm clearance margins</a> is the usual block we recomment. It has 0.2mm gap around all components to provide a slip fit. If your printer or slicer is not well calibrated, you may benefit from the larger clearances. 

Dynamic preview of stl for download:

<div id="stl_cont" style="width:500px;height:500px;margin:1"></div>>

<script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont"), 
      {
          allow_drag_and_drop: false,
          auto_rotate:true,
          auto_resize:true,
          models: 
          [ 
            {filename:"../stls/Assembly%20Jigs/soldering_jigV5-0.2mm_margin.stl", color:"#1E73BE", scale:3, rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
</script>  
- - -  
Community discussion and support is available as a subgroup to the <a href='https://discord.gg/jfnVrUx2uK'>CroXY Discord</a> <a href='https://discord.gg/jfnVrUx2uK'> <img src="images\CroXYDiscord.png" alt="CroXY Discord"></a>


