---
title: "Euclid Probe Deployment Planning"
keywords: assembly planning
tags: [assembly, planning]
last_updated: January 29, 2022
permalink: 01_preflight.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Euclid Probe Assembly Planning 
---
## TL:DR 
Determine the best orientataion of the tool board and probe before assembly. 

The orientation of the tool board does not nescessarily have to match the orientation of the probe. 

The probe is designed to enter the dock like an arrow, the wider section self-centerting the PCB in case of misalignment. 

The 'arrows' can point in opposite ways. In fact, this is the orientaion for an i3 style printer like an Ender3 or Wanhao i3, where the mount points to Xmin and the probe enters the moving dock towards Xmax.   

Guide blocks used to aid in the assembly and for hole drilling and tap aligning are <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/stls/Assembly%20Jigs' target="_blank"> here.</a> They are not required but helpful to users who are not confident in their assembly skills. 

<a href='https://github.com/nionio6915/Euclid_Probe/raw/main/stls/Assembly%20Jigs/soldering_jigV5-0.2mm_margin.stl'>Solder and Drilling Jig with 0.2mm clearance margins</a> is the usual block we recomment. It has 0.2mm gap around all components to provide a slip fit. If your printer or slicer is not well calibrated, you may benefit from the larger clearances. 

Dynamic preview of stl for download:

test link to github   

<div id="stl_cont" style="width:500px;height:500px;margin:1"></div>>
<script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont"), 
      {
          auto_rotate:true,
          auto_resize:true,
          models: 
          [ 
            {filename:'https://github.com/nionio6915/Euclid_Probe/raw/main/stls/Assembly%20Jigs/soldering_jigV5-0.2mm_margin.stl', color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
</script>



- - - 

Community discussion and support is available as a subgroup to the <a href='https://discord.gg/jfnVrUx2uK'>CroXY Discord</a> <a href='https://discord.gg/jfnVrUx2uK'> <img src="images\CroXYDiscord.png" alt="CroXY Discord"></a>


