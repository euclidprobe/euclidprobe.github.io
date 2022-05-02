---
title: "Euclid Probe Mounts"
keywords: probe dock, tool mount
tags: [mounts]
last_updated: January 28, 2022
permalink: 02_mounts.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Euclid Probe Docks & Probes 
---

### Modular Toolboard Mounts

The modular building blocks provided are meant to be integrated into users own printer and other CNC machine designs. They are provided in surface mounted and recessed configurations, with pilot holes for M2.5 self tapping screws, M3 tap pilot holes and bores for M3 heatserts. 

<div style="width:100%;text-align:center;">
 <a href="images\02_Modular_Parts.png" data-lity>
        <img src="images\02_Modular_Parts.png" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>

<a href="https://github.com/nionio6915/Euclid_Probe/raw/main/CAD/Building_Blocks/Modular_PartsV2.zip"><b>Building Blocks as .stp file</b></a>  

<a href=" https://github.com/nionio6915/Euclid_Probe/tree/main/stls/Building%20Blocks" target="blank"><b>Individual Modular parts as stl's</b></a>  

### PCB Board Dimensions  
<div style="width:100%;text-align:center;">
 <a href="images\01-board-dims.png" data-lity>
        <img src="images\01-board-dims.png" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>

### Probe Solid Model  
<div style="width:100%;text-align:center;">
 <a href="images\02_ProbeV4_model1.jpg" data-lity>
        <img src="images\02_ProbeV4_model1.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>   

<div style="width:100%;text-align:center;">
 <a href="images\02_ProbeV4_model2.jpg" data-lity>
        <img src="images\02_ProbeV4_model2.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>  

<a href="https://github.com/nionio6915/Euclid_Probe/raw/main/CAD/ProbeV4_stp.zip"><b>Probe Assembly as a solid model, .stp format </b></a>  

<a href="https://github.com/nionio6915/Euclid_Probe/raw/main/CAD/ProbeV4_dxf.zip"><b>Probe Assembly as a solid model, .DXF format </b></a>  


**December 6, 2021:** We are reorganizing and consolidating the file repo’s. All file download links will be deleted and replaced as we update the webpages. If a download link is missing, users are encouraged to grab the <a href=" https://github.com/nionio6915/Euclid_Probe/tree/main/stls/" target="blank">current files hosted at github</a>

The toolboard was designed to locate the clearance hole for the JST-XH socket far enough away from common sized M3 heatserts so that a reasonable wall thickness could be maintained in 3D printed mounts.

<img src="images\03-MOUNT-MINWALL-1024x620.jpg">  

### 5015 Fan Mount
The 5015 Fan mount prints in 2 halves. Each half is different by design.
There is 1.5mm added clearance in the LeftP1.5 part for a sheet metal bracket if your printer uses one. If the sheet metal bracket is on the right, mirror both parts in your slicer.
The LeftV4 .stl has 0 side clearance.

The RightV4 .stl has 0 side clearance.
There are +5/-2mm vertical adjustment in the mount as shown.

There are +5/-2mm vertical adjustment in the mount as shown.

### 4020 Fan Mount
The 4020 fan mount prints in 2 halves. Each half is different by design.
There is 1.5mm added clearance in the Left part for a sheet metal bracket if your printer uses one. If the sheet metal bracket is on the right, mirror both parts in your slicer. If your printer does not have a sheet metal bracket, an M3 washer will take up the gap.
The Right .stl has 0 side clearance.
There are +5/-2mm vertical adjustment in the mount as shown.

<hr> 

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c6q4{font-family:inherit;text-align:left;vertical-align:top}
.tg .tg-m7tf{background-color:#212830;font-family:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-cjf2{background-color:#212830;text-align:left;vertical-align:top}
</style>
### Modular Toolboard Mounts
<table class="tg">
<thead></thead>
<tbody>
  <tr>
    <th class="tg-m7tf"><img src="images\03-Grafting_Mount2-300x290.png " width="325" height="325"></th>
    <th class="tg-m7tf"><img src="images\03-GraftingDockFlush-256x300.jpg " width="325" height="325"></th>
  </tr>
  <tr>
    <td class="tg-c6q4"><a href='https://github.com/nionio6915/Euclid_Probe/raw/main/stls/Building%20Blocks/Grafting_MountM2Holes.stl'>Grafting Dock for Surface Mount<br>
    M2 Self Tapping Version</a> <br>
    Other versions (M3 Tapping, M3 Heatsert on github repo </td>
    <td class="tg-c6q4"><a href='https://github.com/nionio6915/Euclid_Probe/raw/main/stls/Building%20Blocks/Grafting_MountM2Holes_Recessed.stl'>Grafting Dock for Flush Mount<br>
    M2 Self Tapping Version</a> <br>
    Other versions (M3 Tapping, M3 Heatsert on github repo</td>
  </tr>
  
<tr>
    <td class="tg-0pky">
    <div id="stl_cont0" style="width:250px;height:350px;margin:3"></div>
    <script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont0"), 
      {
          allow_drag_and_drop: false,
          auto_rotate:true,
          auto_resize:false,
          zoom:150,
          models: 
          [ 
            {id:0, filename:"../stls/Building Blocks/Grafting_MountM2Holes.stl", color:"#1E73BE", scale:2,rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
</script>
</td>
    <td class="tg-0pky">
        <div id="stl_cont1" style="width:250px;height:350px;margin:3"></div>
        <script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont1"), 
      {
          allow_drag_and_drop: false,
          auto_rotate:true,
          auto_resize:false,
          zoom:150,
          models: 
          [ 
            {id:1, filename:"../stls/Building Blocks/Grafting_MountM2Holes_Recessed.stl", color:"#1E73BE", scale:2,rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
</script>
</td>
  </tr>


  <tr>
    <td class="tg-m7tf"><img src="images\03-5015FanMount-1-220x300.jpg "></td>
    <td class="tg-m7tf"><img src="images\03-5015FanMount-2-241x300.jpg "></td>
  </tr>
  <tr>
    <td class="tg-0lax">5015 Fan Mount</td>
    <td class="tg-0lax">5015 Fan Mount</td>
  </tr>
  <tr>
    <td class="tg-cjf2"><img src="images\03-4020Fan01-268x300.jpg"></td>
    <td class="tg-cjf2"><img src="images\03-4020Fan02-274x300.jpg "></td>
  </tr>
  <tr>
    <td class="tg-0lax">4020 Fan Mount</td>
    <td class="tg-0lax">4020 Fan Mount</td>
  </tr>
</tbody>
</table>
