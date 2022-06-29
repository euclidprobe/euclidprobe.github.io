---
title: "Voron Overview"
keywords: Voron
tags: [mounts, docks]
last_updated: February 5, 2022
permalink: 02c_Voron.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Voron Probe Docks & Mounts Overview 
---

## Mounts & Docks for Voron
Below is a general summary for Voron printers. More specific information on the individual model pages. 

Screen snips, CAD's and stl's in are <a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/" targer="blank">in the github repo</a> and linked from the individual pages. 

Voron printers can utilize the Omton/Fotek conversion mount for existing builds. 

Modified carraige shells (both MGN9 & MGN 12 versions) locate the toolboard in the same realtive (X,Y) location as the inductive probe, but ~4.5mm higher. 

{% include note.html content="Using conversion mounts offers the most flexibility and fine tuning of probe height." %}

{% include note.html content="<b>No implementation to Stealthburner / CW2 has been made. When we asked the point person on the Voron design team, (aka the person with the authority to release them, and whom we respect)  for the CAD's to work on Euclid adaptations, told us that the official position is they are not ready to be released and that we will be notified when they are officially released.   

We are honoring his response because it is the correct and right thing to do.  
.</b>" %}


## Clcockwork1 - 2xMGN9 Rail & MGN12 - Afterburner Native Mounts
The left and right halves of the Afterburner carriage are modified to accept the probe with M3 screws and heatserts or M2.5 self tapping screws from underneath. Fine tuning and tweaking credited to garbqgebag.  

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
The standard Omron mount is 0 degree relative rotation to the mounting face of the Omron device. Adjustment slots are similar to the original device.  Designed to be printed upside-down without supports.  Screens are out of date, but the stls and CAD models are updated

<div style="width:100%;text-align:center;"> <a href="stls\Omron\02_OmronFotec.png" data-lity>
<img src="stls\Omron\02_OmronFotec.png" style="height:315px; border:2px solid CornflowerBlue"></a>  

 <a href="stls\Omron\02_OmronFotec90.png" data-lity>
<img src="stls\Omron\02_OmronFotec90.png" style="height:315px; border:2px solid CornflowerBlue"></a>  
</div>  

Omron Mounts are <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/stls/Mount%20Adapters/Omron' target="_blank"><b> here.</b></a>

## Skinny Mount- Improved Airflow mount by v6cl 
Github user v6cl posted a video to Youtube that we came across and we were impressed by their deployment. They designed a ‘skinny mount’ to  <a href="https://github.com/v6cl/My-Voron2.4-Customs/tree/main/euclid_mount_slim" targer="blank">open up the cooling vents in the toolhead.</a>

<div style="width:100%;text-align:center;"> <a href="images\02-voron\v6cl.png" data-lity>
<img src="images\02-voron\v6cl.png" style="height:315px; border:2px solid CornflowerBlue"></a>  

 <a href="images\02-voron\v6cl_dtl.png" data-lity>
<img src="images\02-voron\v6cl_dtl.png" style="height:315px; border:2px solid CornflowerBlue"></a>  
</div>  
<br>  

Their repo is at <a href="https://github.com/v6cl/My-Voron2.4-Customs">https://github.com/v6cl/My-Voron2.4-Customs</a>  

## Stealthburner 
We are waiting for the official Voron release to implement our adaptations to Stealthburner. 

When we asked the Voron developers for source files to work on our adaptations, they asked us to wait for their official release and we are honoring their request.  


## Trident & 2.4 Native Gantry Dock & Mount 

The mount attaches with screws in the holes of the left side motor bracket and clears the radius of the cable chain. M5x16 & M5x30's  
     
The dock attaches to the mount with an M5 nut dropped in the keyholed channel and thru-bolts with an M5x16 screw. Adjust the elevation as required to allow for a clean exit of the probe PCB. Fine tuning and tweaking credited to Dattas and StvPtrsn.

<div style="width:100%;text-align:center;">
<a href="images\02-voron\Trident_TopMount.png" data-lity>
<img src="images\02-voron\Trident_TopMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Trident_TopMountXRay.png" data-lity>
<img src="images\02-voron\Trident_TopMountXRay.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Trident_TopMountXRay2.png" data-lity>
<img src="images\02-voron\Trident_TopMountXRay2.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
</div> 

## Straight Armed Gantry Dock & Mount
This mount attaches to the rear extrusion of the gantry, in the native holes of the left side motor bracket. Requires the use of the Omron90 mount. Lateral adjustment buy the thru-bolt on the bottom, M5x16. Fine vertical adjustment via the slotted holes in the Omron mount. 

This probe orientation / configuration should be compatible with the other detachable probe macros for Voron. 

<div style="width:100%;text-align:center;">
<a href="images\02-voron\Voron2.4_XRailMount2.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount2.png" style="height:250px; border:2px solid CornflowerBlue"></a>  

<a href="images\02-voron\Voron2.4_XRailMount.png" data-lity>
<img src="images\02-voron\Voron2.4_XRailMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
</div>

## 90 Degree Gantry Dock & Mount
This dock is orientated in the X direction and attaches to the rear extrusion of the gantry, in the native holes of the left side motor bracket. Requires the use of the Omron90 mount. Attaches with longer screws. Lateral Y adjustment via the thru-bolt on the bottom, M5x16. Fine vertical adjustment via the slotted holes in the Omron mount or with shims between the Y adjuster.   

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

