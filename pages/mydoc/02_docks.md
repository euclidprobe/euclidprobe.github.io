---
title: "Euclid Probe Docks"
keywords: probe dock, tool mount
tags: [docks]
permalink: 02_docks.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Euclid Probe Docks 
---

### Determine the best orientation of the tool board and probe before assembly.

The orientation of the tool board does not necessarily have to match the orientation of the probe. 

The probe is designed to enter the dock like an arrow, the wider section self-centering the PCB as it enters in case of any misalignment. 

<div id="pic0" style="width:500px; margin:3">
<img src="images\02_dock_entry.jpg"><br>  
</div>  


The 'arrows' can point in opposite ways. In fact, this is the orientation for an i3 style printer like an Ender3 or Wanhao i3, where the tool board motion points it to Xmin and the probe entering the Y-moving dock towards Xmax.   

<div id="pic0" style="width:500px; margin:3">
<img src="images\02_Ender3_probe_dock.jpg"><br>  
</div>  

###  Locating the Probe Dock
Printer mounted docks are needed for automatic deployment and retraction. Depending on the firmware's gcode programming capabilities, the dock can be either fixed frame or moving bed mounted.

The best place to put the dock is in a area that is outside of the printing boundary – the overrun area where things like purge buckets, nozzle wipers, tool docks, etc… live. This is the perfect location for Euclid’s dock.   

If your printer does not have such an area, then an area roughly 15mm x 30mm in X & Y needs to be dedicated for the dock.  It might sound worse than it is- even in the toughest adaptation, the max loss to print area was 4mm x 15mm. 

The best advice we can offer is to look at the adaptations that are published in the .stls and CAD folder for inspiration. 

The ideal location provides for both in and out motion of the probe into the dock, and as well a swiping action perpendicular to the dock to strip the probe from the toolboard.  

Most often, this location ends up being in one of the back corners of any X-Y type machines. 

On deltas style printers, the dock ideally mounts next to one of the rear towers.  

Keep the dock and the dock mount as short as possible so it's as stiff as possible.

## Servo actuated docks & Linear stages
Docks attached to compound levers or bellcrank actuated mechanisms have performed better than direct attached docks to servo arms. These setups work, but we don't currently have the resources to develop. 

Here is an example of Jay_s' servo setup on his Voron V0.1:  
<div style="width:100%;text-align:center;"> 
<a href="https://www.youtube.com/watch?v=wlnXIud-uro" data-lity>  
<img src="images\03_jays_servo.png" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div>

Here is an example of an inexpensive linear stage with 50mm of travel moving the dock into the print area and retracting it. IT uses a NEMA11 motor, leadscrew and a section of ball bearing rail to provide repeatable controlled motion. 
<div style="width:100%;text-align:center;"> 

<a href="https://smile.amazon.com/Befenybay-Effective-Travel-Stepper-Actuator/dp/B087NMCGPV" target="blank"> Linear stage at Amazon Example</a>  <br>

<a href="images\02_linear_stageB.jpg" data-lity>
<img src="images\02_linear_stageB.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>

<a href="https://www.youtube.com/watch?v=IKLWkvJxWOw" data-lity>
<img src="images\02_linear_stage.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>  

</div>

#### Setting the Probe Dock Height
The elevation of the dock is critical for consistent, problem free deployment and retraction.

The ideal probe dock and toolboard designs allow for adjustments of the dock vertically so that when the probe is in the dock, it can meet the toolboard and be raised by the magnets to the proper elevation to clear the exit gate.

<div style="width:100%;text-align:center;"> <a href="images\02_Dock_Height_2.jpg" data-lity>
<img src="images\02_Dock_Height_2.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>

<a href="images\02_Dock_Alignment.jpg " data-lity>
<img src="images\02_Dock_Alignment.jpg" style="width:400px; border:2px solid CornflowerBlue"></a></div>  

<div style="width:100%;text-align:center;"> <a href="images\02_Front-Probe.png " data-lity>
<img src="images\02_Front-Probe.png " style="width:400px; border:2px solid CornflowerBlue"></a>

<a href="images\02_Front-Undocked.png " data-lity>
<img src=" images\02_Front-Undocked.png" style="width:400px; border:2px solid CornflowerBlue"></a></div>

### Printing the Dock
The usual probe dock is meant to be printed in an upright orientation with the print in place supports under the shoulder that the probe rests against when docked. 

The version with a registration boss is provided to key into another part and to provide for some lateral adjustment. It is sized for an M3 screw as a draw bolt. The size of the boss is 6mm high by 1.5mm deep.

### What are the holes for?
The vertical hole in the top of the dock was originally intended to provide a pocket for either a cylinder magnet or steel screw to provide something for the front magnet to attract to and retain the probe. Through testing, it was determined that neither is required. 

However, this hole has been left in place to provide a space for a HALL effect sensor to be inserted and act as a visual indicator or part of a probe detection circuit. This will be covered in later sections.  

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-1ono{background-color:#212830;border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-znyc{background-color:#212830;border-color:inherit;font-family:inherit;font-size:100%;text-align:left;vertical-align:top}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-1ono"><img src='images\02_ProbeDockPIP_201x300.jpg' alt="IMG1" width="500" height="400"></th>
    <th class="tg-1ono"><img src="images\02_ProbeDockRegBossPIP_201x300.jpg" alt="IMG2" width="500" height="400"></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky"><a href='https://github.com/nionio6915/Euclid_Probe/raw/main/stls/Building%20Blocks/Grafting_DockV3.stl'>  Modular Grafting Dock .stl</a></td>
    <td class="tg-0pky"> <a href='https://github.com/nionio6915/Euclid_Probe/raw/main/stls/Building%20Blocks/Grafting_Dock_RegBoss_V3.stl'>  Modular Grafting Dock<br/>with Registration Boss .stl</a> </td>
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
            {id:0, filename:"../stls/Building Blocks/Grafting_DockV3.stl", color:"#1E73BE", scale:2,rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
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
            {id:1, filename:"../stls/Building Blocks/Grafting_Dock_RegBoss_V3.stl", color:"#1E73BE", scale:2,rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
</script>
</td>
  </tr>
</tbody>
</table>

---  
Community discussion and support is available as a subgroup to the <a href='https://discord.gg/jfnVrUx2uK'>CroXY Discord</a> <a href='https://discord.gg/jfnVrUx2uK'> <img src="images\CroXYDiscord.png" alt="CroXY Discord"></a>

