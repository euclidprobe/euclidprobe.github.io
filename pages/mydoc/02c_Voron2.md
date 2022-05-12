---
title: "Voron Overview"
keywords: Voron
tags: [mounts, docks]
last_updated: February 5, 2022
permalink: 02c_Voron2.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Voron Probe Docks & Mounts Overview 
---

## Mounts by Printer Voron
Existing Voron 2.4’s can utilize the Fotek converstion mount or the modified AfterBurner shells offered below which locate the toolboard in the same location as the inductive probe.  

Github user v6cl posted a video to Youtube that we came across and were impressed by their deployment. They designed a ‘skinny mount’ to open up the cooling vents in the toolhead.  

## Clcockwork1 - 2xMGN9 Rail & MGN12 - Afterburner Native Mounts
The left and right halves of the Afterburner carriage are modified to accept the probe with M3 screws and heatserts from underneath. Fine tuning and tweaking credited to garbqgebag.  Images are for the MGN12 version, but stl's and CAD files for both available.   

<div style="width:100%;text-align:center;">
<a href="images\02-voron\afterburner-1.8.png" data-lity>
<img src="images\02-voron\afterburner-1.8.png" style="height:250px; border:2px solid CornflowerBlue"></a>

<a href="images\02-voron\Voron_Afterburner-Native.png" data-lity>
<img src="images\02-voron\Voron_Afterburner-Native.png" style="height:250px; border:2px solid CornflowerBlue"></a>

<a href="images\02-voron\image1.jpg" data-lity>
<img src="images\02-voron\image1.jpg" style="height:250px; border:2px solid CornflowerBlue"></a>

<a href="images\02-voron\image2.jpg" data-lity>
<img src="images\02-voron\image2.jpg" style="height:250px; border:2px solid CornflowerBlue"></a>
</div>  

## Omron Mounts  
The standard Omron mount is 0 degree relative rotation to the mounting face of the Omron device. Adjustment slots are similar to the original device.  Designed to be printed upside-down without supports.  Dock entry is in the X axis. 

The Omron90 mount includes a 90 degree relative rotation to the mounting face. Adjustment slots are similar to the original device.  The orientation is to utilize docking and undocking motions in the Y axis orientation for those upgrading from other devices to maintain the 
existing macros. Designed to be printed upside-down without supports.  

<div style="width:100%;text-align:center;"> <a href="stls\Omron\02_OmronFotec.png" data-lity>
<img src="stls\Omron\02_OmronFotec.png" style="height:315px; border:2px solid CornflowerBlue"></a>  

 <a href="stls\Omron\02_OmronFotec90.png" data-lity>
<img src="stls\Omron\02_OmronFotec90.png" style="height:315px; border:2px solid CornflowerBlue"></a>  
</div>  

Omron Mounts are <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/stls/Mount%20Adapters/Omron' target="_blank"><b> here.</b></a>   

## Clockwork2 Native Mounts  
We are waiting for the official release of Clockwork 2 to release our native Afterburner Mounts. 


## Clockwork1 Native Docks & Dock Mounts  
### Gantry Mount 
Version 4 of the gantry mount adjustable in height. It should place the dock at X0 Ymax location. This mount is intended to utilize the Omron adapter to fine tune the height of the probe into the dock.  

<div style="width:100%;text-align:center;">
<a href="images\02-voron\GantryMountV4.png" data-lity>
<img src="images\02-voron\GantryMountV4.png" style="height:250px; border:2px solid CornflowerBlue"></a>
</div>  


Version 2 SHORT of the gantry mount is fixed in height and location and is for users of the native carriage shells.It requires the use of shims to provide fine tuning of the probe height. 

A recess for either a 6x3 magnet or M3 nut has been provided in the nose of the dock to server as a keeper for the probe.  

This mount attaches through and clamps the left side motor mount bracket with an M5x16 and M5x30 screw from the BOM.   This was developed with the collaboration of Discord users Dattas, Deepsiks, Kyleisah and StvPtrsn.

<div style="width:100%;text-align:center;">
<a href="images\02-voron\VoronGantryMountRev2.jpg" data-lity>
<img src="images\02-voron\VoronGantryMountRev2.jpg" style="height:250px; border:2px solid CornflowerBlue"></a>
</div>  

<div style="width:100%;text-align:center;">
<table>
<tr>
<td>
<div id="stl_cont00" style="width:450px;height:450px;margin:0 auto;">
  <script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont00"), 
      {
          allow_drag_and_drop: false, 
          auto_rotate:true,
          auto_resize:true,
          zoom:200,
          models: 
          [ 
            {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev_4_Set.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
  </script>
</div>  
</td>
<td>
<div id="stl_cont01" style="width:450px;height:450px;margin:0 auto;">
  <script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont01"), 
      {
          allow_drag_and_drop: false, 
          auto_rotate:true,
          auto_resize:true,
          zoom:200,
          models: 
          [ 
            {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev2_Short.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
  </script>
</div>  
</td>
</tr>
<tr>
<td>
  <a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev_4_Set.stl" target="blank">Voron 2.4 and Trident Gantry Mount Version 2</a>  
  </td>
  <td>
  <a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev2_Short.stl" target="blank">Voron 2.4 and Trident Gantry Mount Version 2 Short</a>  
  </td>
  </tr>
  </table>  
  </div>  

### Gantry Mount 90 Degree Probe 
This dock is orientated in the Y direction and attaches to the rear extrusion of the gantry, in the native holes of the left side motor bracket. Requires the use of the Omron90 degree mount. Attaches with longer screws, M5x20. 
Lateral Y adjustment via the thru-bolt on the bottom, M5x16. Fine vertical adjustment via the slotted holes in the Omron90 mount, or with shims between the Y adjuster. 

This configuration should be compatible with the other detachable probe macros for Voron.  

<div style="width:100%;text-align:center;">
<a href="images\02-voron\Voron2.4_XRailMount2.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount2.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Voron2.4_XRailMount.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
</div>

## Voron 2.4 Bed Rail Mounted Dock  
The bed mounts are provided in 2 heights to suit the overall stack height of the bed plate and printing surfaces. This dock has been tested by multiple users. Fine tuning and tweaking credited to kageurufu.  

The stls are provided to print 'nose' down and have minimal print in place supports to ensure that the back shoulder is printed and aligned.  

The bed rail mount uses 2-M5x16 screws and extrusion nuts to attach to either side of the extrusions that support the bed.  

There are 2 hex-shaped cross holes to the main mounting screws- these are provide to insert M3 screws to use as fine adjusters without tapping. They can be M3 setscrews and left in place or any M3 screw used temporarily.   
<div style="width:100%;text-align:center;">
<a href="images\02-voron\VVoronBedPArtial.jpg" style="height:250px; border:2px solid CornflowerBlue"></a>

<a href="images\02-voron\Voron2.4BedMount.png" data-lity>
<img src="images\02-voron\Voron2.4BedMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Voron2.4BedMount.png" data-lity>
<img src="images\02-voron\Voron2.4BedMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
</div>   

## CAD Files
The current CAD files are <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/CAD' target="_blank"><b> available here in the repo.</b></a>