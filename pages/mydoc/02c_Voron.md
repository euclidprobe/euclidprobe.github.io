---
title: "Voron Overview"
keywords: Voron
tags: [mounts, docks]
last_updated: February 5, 2022
permalink: 02c_Voron.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Voron Probe Docks & Mounts Overview 
---

## Mounts by Printer Voron
Page currently undergoing maintenance. 
Screen snips and stls in are <a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/">in the github repo</a>

Existing Voron 2.4’s can utilize the Fotek converstion mount or the modified AfterBurner shells offered below which locate the toolboard in the same location as the inductive probe.

Github user v6cl posted a video to Youtube that we came across and were impressed by their deployment. They designed a ‘skinny mount’ to open up the cooling vents in the toolhead.

# Repository of stl's for Voron printers

## Clcockwork1 - 2xMGN9 Rail & MGN12 - Afterburner Native Mounts
The left and right halves of the Afterburner carriage are modified to accept the probe with M3 screws and heatserts from underneath. Fine tuning and tweaking credited to garbqgebag.  

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
The standard Omron mount is 0 degree relative rotation to the mounting face of the Omron device. Adjustment slots are similar to the original device.  Designed to be printed upside-down without supports.  

<div style="width:100%;text-align:center;"> <a href="stls\Omron\02_OmronFotec.png" data-lity>
<img src="stls\Omron\02_OmronFotec.png" style="height:315px; border:2px solid CornflowerBlue"></a>  

 <a href="stls\Omron\02_OmronFotec90.png" data-lity>
<img src="stls\Omron\02_OmronFotec90.png" style="height:315px; border:2px solid CornflowerBlue"></a>  
</div>  

Omron Mounts are <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/stls/Mount%20Adapters/Omron' target="_blank"><b> here.</b></a>


## Clockwork2 Native Mounts  
We are waiting for the official release of Clockwork 2 to release our native Afterburner Mounts. 


## Clockwork2 Native Dock & Mount  
The mount attaches with longer screws in the holes of the left side motor bracket and clears the radius of the cable chain. 3-M5x20 screws required.  
     
The dock attaches to the mount with an M5 nut dropped in the keyholed channel and thru-bolts with an M5x20 screw. Adjust the elevation as required to allow for a clean exit of the probe PCB. Fine tuning and tweaking credited to Dattas.

<div style="width:100%;text-align:center;">
<a href="images\02-voron\Trident_TopMount.png" data-lity>
<img src="images\02-voron\Trident_TopMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Trident_TopMountXRay.png" data-lity>
<img src="images\02-voron\Trident_TopMountXRay.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Trident_TopMountXRay2.png" data-lity>
<img src="images\02-voron\Trident_TopMountXRay2.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
</div> 

## Gantry Dock & Mount
This mount attaches to the rear extrusion of the gantry, attaches with longer screws, M5x16, in the native holes of the left side motor bracket. Requires the use of the Omron90 mount. Lateral adjustment bu the thru-bolt on the bottom, M5x16. Fine vertical adjustment via the slotted holes in the Omron mount. Currently untested and unproven to our knowledge- please contact us if difficulties are encountered.  
This configuration should be compatible with the other detachable probe macros for Voron. 

<div style="width:100%;text-align:center;">
<a href="images\02-voron\Voron2.4_XRailMount2.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount2.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Voron2.4_XRailMount.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
</div>

## 90 Degree Gantry Dock & Mount
This dock is orientated in the X direction and attaches to the rear extrusion of the gantry, in the native holes of the left side motor bracket. Requires the use of the Omron90 mount or Native Afterburner Carriage. Attaches with longer screws, M5x16, . Lateral Y adjustment via the thru-bolt on the bottom, M5x16. Fine vertical adjustment via the slotted holes in the Omron mount or with shims between the Y adjuster. Currently untested and unproven to our knowledge- please contact us if difficulties are encountered. This configuration should be compatible with the other detachable probe macros for Voron.  
<div style="width:100%;text-align:center;">
<a href="images\02-voron\Voron2.4_XRailMount90.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount90.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Voron2.4_XRailMount90a.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount90a.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
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

