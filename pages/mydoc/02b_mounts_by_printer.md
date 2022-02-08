---
title: "Modular Docks & Mounts"
keywords: probe dock, tool mount
tags: [mounts, docks]
last_updated: January 24, 2022
permalink: 02b_mounts_by_printer.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Euclid Probe Docks & Probes 
---

###  Repository of stl's for probe adapters and probe docks 

<a href='https://github.com/nionio6915/Euclid_Probe/tree/main/CAD' target="_blank"><b>
CAD files in the CAD directory.</b></a> &nbsp;&nbsp;&nbsp;  <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/CAD' target="_blank"><b> stl's in the stl's directory </b></a>   

Provided Docks and adapters are designed to be printed at either 0.2mm or 0.3mm layer heights. Some probe dock stl's are offered with both Print In Place supports and without. We attempt to provide the files in the best orientation for printing, but users are recommended to verify against their best print settings. 

**February 6, 2022:** We are reorganizing and consolidating the file repo’s. All file download links will be deleted and replaced as we update the webpages in the sidebar menu.  
If a download link is missing, users are encouraged to grab the current files hosted at github linked above.  
We apologize for the maintenance.  

The best probe deployment results seem to be had by printing the probe dock with the the exit gate at the bottom, or by printing it with the gate at the top with the internal supports supporting the shoulder the PCB stops against. 

If the dock must be printed laying flat, it is recommended that top surface of your print be the underside of the dock.  This orientation allows the PCB to bear against the 'best top of print surface' of the dock.  The bottom of the well surface can be a little rough and uneven resulting from support structures.  

Note: there is a 5x5mm pocket to insert an optional magnet or ferrous object to retain the probe in the dock. It is not required. This was utilized in early stages of development and remains a legacy for now. 

**The design of your dock is critical to the successful attaching and detaching of the probe.** 
The Euclid Probe dock utilizes a well, so that when the probe is stripped from the carriage, it is retained by the stops. Upon probe pickup, the probe PCB must clear the exit gates/slots. Adjust the elevation of either the carriage in the deployment gcode or adjust the dock so that in the coupled condition, the probe will slide out without interference.   

### Examples of provided Mounts & Docks  
**BLTouch Adapter Mount**
<div style="width:100%;text-align:center;"> 
<a href="stls\BLTouch\02_BLTV3.jpg" data-lity>
<img src="stls\BLTouch\02_BLTV3.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div>  

**Ender3 Mount**
<div style="width:100%;text-align:center;"> 
<a href="images\EnderDock.jpg" data-lity>
<img src="images\EnderDock.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>  
<a href="images\EnderMount.jpg" data-lity>
<img src="images\EnderMount.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div>  

**Ender5 Mount**
<div style="width:100%;text-align:center;"> 
<a href="images\02_Ender5.jpg" data-lity>
<img src="images\02_Ender5.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div>  


**Fixed Frame Dock**
2 Piece design, uses M3 screws and captive nuts to couple the parts. Vertical slots in the mount provide adjustability.  
<div style="width:100%;text-align:center;"> 
<a href="images\old_github\02_Probe_Dock_Fixed.png" data-lity>
<img src="images\old_github\02_Probe_Dock_Fixed.png" style="width:300px; border:2px solid CornflowerBlue"></a>
<a href="images\old_github\02_Probe_Docked.png" data-lity>
<img src="images\old_github\02_Probe_Docked.png" style="width:300px; border:2px solid CornflowerBlue"></a>
</div> 

**Movable Bed Dock**  
Uses long style, double taper heatserts for assembly. Mounts to the end of a 2020 bed support rail and is adjustable for height. Allows for interchangeble beds to fit under the mount. Requires a change the Z probe offset constant by the bed thickness on the fly. ( G31 Z-(bed thickness) )     
<div style="width:100%;text-align:center;"> 
<a href="images\old_github\02_2020Rail_Mount.png" data-lity>
<img src="images\old_github\02_2020Rail_Mount.png" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div> 

**Omron / Fotec Adapter mount**   
<div style="width:100%;text-align:center;"> 
<a href="stls\Omron\02_OmronFotec.png" data-lity>
<img src="stls\Omron\02_OmronFotec.png" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div> 

**Railcore Dock & Carriage Adapter**  
Railcore clip-on dock is a 2 piece design for adjustability, still under development due to all the variations of Railcore design. 
The Railcore carriage mounts are available in three versions- the Original Design/713Maker geometry, the MRW geometry, and Petsfang Colling Shroud mount.  

<div style="width:100%;text-align:center;"> 
<a href="images\02_RC_Corner.jpg" data-lity>
<img src="images\02_RC_Corner.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>  
<a href="" data-lity>
<img src="" style="width:300px; border:2px solid CornflowerBlue"></a>  
<a href="images\02_RC_Mount.jpg" data-lity>
<img src="images\02_RC_Mount.jpg" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div> 


**V-Core3 & EVA Carriage**  
<div style="width:100%;text-align:center;"> 
<a href="images\02_EVA_Mount" data-lity>
<img src="images\02_EVA_Mount" style="width:300px; border:2px solid CornflowerBlue"></a> 

<a href="images\02_VCore" data-lity>
<img src="images\02_VCore" style="width:300px; border:2px solid CornflowerBlue"></a> 

<a href="images\02_VCoreB" data-lity>
<img src="images\02_VCoreB" style="width:300px; border:2px solid CornflowerBlue"></a> 
</div> 



**Voron Afterburner V4 Mod**  
Recessed mount for Euclid probe in the the bottom of the carriage parts, pushing the probe further back in Y direction. 
<div style="width:100%;text-align:center;"> 
<a href="images\02_Voron_Afterburner-Native.png" data-lity>
<img src="images\02_Voron_Afterburner-Native.png" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div> 


**Voron 2.4 Frame Mount**  
This mount mounts to the main frame of the printer. Users are cautioned that the probe will always be in the plane of the motion system, and there is always a possibility of errant probe pickup compared to the bed mounted dock below.   
<div style="width:100%;text-align:center;"> 
<a href="images\02_Voron2.4_XRailMount90.png" data-lity>
<img src="images\02_Voron2.4_XRailMount90.png" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div> 


**Voron 2.4 Bed Rail Mount**
This mount attaches to the print bed mounting rail. The potential for errant probe pickup is reduced to the Z elevation of the magnet strengths.   
<div style="width:100%;text-align:center;"> 
<a href="images\02_Voron2.4BedMount.png" data-lity>
<img src="images\02_Voron2.4BedMount.png" style="width:300px; border:2px solid CornflowerBlue"></a>  
</div> 

