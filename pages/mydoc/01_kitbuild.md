---
title: "Euclid Probe Kit Instructions"
keywords: assembly 
tags: [assembly]
permalink: 01_kitbuild.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Euclid Probe Kit Instructions 
---

## Build Instructions

Reminder that community discussion and support is available as a subgroup to the <a href='https://discord.gg/jfnVrUx2uK'>CroXY Discord</a> <a href='https://discord.gg/jfnVrUx2uK'> <img src="images\CroXYDiscord.png" alt="CroXY Discord"></a>
<hr>
### TL:DR 
Open the bag carefully; sort your parts: solder the header and switch; attach your magnets; screw the toolboard to the mount; attach your dock; config your FW; print happily ever after!

### Step 1 – Board Preparation:
The Euclid Probe kit will arrive in a small zip-sealed baggie. Beware, there are small parts that can be easily lost.

<img src="images\01_assembly\baggie-300x202.jpg">  

The kit contains the PCB set, screws, SMD nuts, a switch, magnets and wiring connectors.  

<img src="images\01_assembly\01_kit_contents.jpg">  

Leave the two PCB’s attached to the rail for now. It will aid in the solder assembly of the components.  

Determine the orientation for the plunger on the switch:
 -  Most installations will favor the plunger to the rear of the probe. That way the eccentricity between the nozzle and plunger is minimized. The COM-NC pins on the switch correspond to the holes on the PCB labeled COM and NC.  
 -  <img src="images\01_assembly\01-switch_pins.jpg">  
 -  <img src="images\01_assembly\01_plunger_bias_rear.jpg">  

 -  Installations on printers like Ender3 will benefit from the plunger towards the front of the probe.  

 -  <img src="images\02_Ender3_probe_dock.jpg">  
 -  <img src="images\01_assembly\01_plunger_bias_front.jpg">  

Determine how you will be attaching the upper tool board PCB to your carriage. The mount holes in the upper board are drilled thru 2.5mm⌀:
    - Use the included M2.5x6 self tapping screws into the pilot holes for the provided mounts.
    - Tap pilot holes for with an M3 tap so that you can secure it from above and have concealed fasteners.
    - Drill through with M3mm⌀ and use M3 screws to secure to M3 heatserts embedded in your carriage. This is a popular method. 
    - Countersink for concealed fasteners. There is sufficient material in the PCB to countersink the screw holes to use flat head screws for a flush installation to threaded holes above.
    - The holes are positioned such that if heatserts were used in a carriage, there will be sufficient cover in the margins between the JST connector housing clearance hole and the inserts.

You may want to print out the combined soldering holder & drill-tap guide block that we have designed. It will hold the JST header and switch upright for soldering and as an aid to align an M3 tap or 3mm⌀ drill perpendicular to the toolboard. The differences in versions are the clearance allowances around the outlines. Print the -3 version if you have a reasonably tuned printer.

### Step 2 - Board Assembly:

The solder jig provided as an aid to hold and align the thru-hole parts. It is not required, but makes for easier assembly. 

Install the wiring connector to upper tool board. This PCB has the outline of the JST-XH socket header printed on the backside and has the surface mounted components installed to the front side. Install the connector from the backside of the board so that all the thru-hole soldering will occur on the front side. The socket header may be interchanged with straight male pins to use the Dupont style connector.
Solder the switch and connector to the PCB boards.

{% include warning.html content="<b>Solder the center pin only so that final adjustments can be made. If the position is too far off, then adjust by reflowing the solder joint.</b>" %}

Install the switch to the probe board with the footprint labeled SW1. Install the switch from the backside. Note the pin labeling on the PCB silk screen printing and align the plunger fore or aft to suit. 

{% include tip.html content="If not using the solder jig, it is helpful to use a dot of superglue to attach the switch and the connector the board before soldering.<br>
The pre-glued components will aid in keeping the PCB’s inverted and stable for hand soldering without a jig." %}

It is important to fully seat the switch against the PCB when soldering. This eliminates any potential lateral movement of the switch due to bending of the soldered pins, maintaining the best possible probe accuracy.

<div style="width:100%;text-align:center;">
<table>
<tbody>
<tr>
    <td> <a href="images\01_assembly\01_solder_jigA.jpg" data-lity>
        <img src="images\01_assembly\01_solder_jigA.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_solder_jigB.jpg" data-lity>
        <img src="images\01_assembly\01_solder_jigB.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
<tr>
    <td> <a href="images\01_assembly\01_solder_jigC.jpg" data-lity>
        <img src="images\01_assembly\01_solder_jigC.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_solder_jigD.jpg" data-lity>
    <img src="images\01_assembly\01_solder_jigD.jpg" style="width:400px; border:2px solid CornflowerBlue">
  </a></td>
</tr>
<tr>
    <td> <a href="images\01_assembly\01_jst_solder.png " data-lity>
        <img src="images\01_assembly\01_jst_solder.png " style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_switch_solder.png" data-lity>
    <img src="images\01_assembly\01_switch_solder.png" style="width:400px; border:2px solid CornflowerBlue">
  </a></td>
</tr>
</tbody>
</table>
</div>
<!-- DivTable.com -->
<div style="width:100%;text-align:center;">
<table>
<tbody>
<tr>
    <td> <a href="images\01_assembly\01_switch-dtl.png" data-lity>
        <img src="images\01_assembly\01_switch-dtl.png" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_jst-dtl.png" data-lity>
        <img src="images\01_assembly\01_jst-dtl.png" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
</tbody>
</table>
</div>


After soldering you can clip the excess length of the solder pins. 

It is suggested to insulate the exposed terminals of the top side of the probe PCB by placing a piece of Kapton tape (not included) or similar non-conductive material to insulate the exposed terminals.  

Nail polish or model builder's enamel works well too.

<div style="width:100%;text-align:center;">
<table>
<tbody>
<tr>
    <td> <a href="images\01_assembly\01_solder_jigF.JPG" data-lity>
        <img src="images\01_assembly\01_solder_jigF.JPG" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_insulate_clipd.jpg" data-lity>
        <img src="images\01_assembly\01_insulate_clipd.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
</tbody>
</table>
</div>


### Step 3 – Magnet Installation
In the kit there are 4, M2x0.4 by 5mm long screws, 4 countersunk magnets and 4 M2 SMD nuts. These are used to secure the magnets to the holders.  

The suggested orientation of the magnets is such that the probe will only couple in one specific orientation by opposing the magnet’s polarities. The magnets area ideally orientated so that their poles alternate fore and aft on the board. 

The photo below shows how we package the magnets in their holders with their polarities and countersinks opposed. The magnets are prevented from pushing out the flat back side of the holder.

<div style="width:100%; text-align:center;">
<a href="images\01_assembly\01_mags_shipping.jpg" data-lity>
<img src="images\01_assembly\01_mags_shipping.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div> 
<br>

We identify the polarities with letters and color codes to aid in installation. The holders also space the magnets the proper distance apart for installation. 

The intent is that the user swivels the holders apart and then inserts the M2 screws thru the countersunk magnet to install.   

The magnets should easily eject from their holders- the direction of magnet ejection is opposite of their insertion. 

<div style="width:100%; text-align:center;">
<a href="images\01_assembly\mag-polarity-768x360.jpg" data-lity>
<img src="images\01_assembly\mag-polarity-768x360.jpg" style="width:400px; border:2px solid CornflowerBlue">
</a></div> 
<br>

This way, when the tool approaches the probe in the dock, the leading magnet’s polarity is opposite of the first. Since these two magnets are of the same polarity, they are repulsed, pushing the probe into the dock and allowing the tool to pass over. When the tool aligns with the second magnet, the probe will be lifted in the dock and couple with the tool.

The solder jig aids in this installation step as well- place the SMD nuts on the jig and place the PCB on back top. You will then be able to put the swiveled magnet holders on top and screws through to attach. 

If not using the jig, place the shoulder of one of the SMD nuts into one of the holes of the PCB from the same side that the switch was installed from. Push the nut fully into the hole and screw the magnet into the nut. 

The SMD nut is shallower than the PCB thickness and tightening the screw will cause the magnet to bear against the plated hole, creating the electrical connection. The magnet should now be protruding on the opposite side of the PCB board from the switch.

{% include warning.html content="<b>Tighten the screw snug tight. Overtightening may result in cracking of the magnets! </b>" %}

<div style="width:100%;text-align:center;">
<table>
<tbody>
<tr>
    <td> <a href="images\01_assembly\01_mag_insertionA.jpg" data-lity>
        <img src="images\01_assembly\01_mag_insertionA.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_mag_insertionB.jpg" data-lity>
        <img src="images\01_assembly\01_mag_insertionB.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
<tr>
    <td> Insert the SMD nuts in the jig.<br>Separate the magnet pairs by swiveling.</td>
    <td> Insert screw through countersunk magnet into trapped SMD nut under PCB board. Tighten snug tight. </td>
</tr>
<tr>
    <td> <a href="images\01_assembly\01_mag_insertionC.jpg" data-lity>
        <img src="images\01_assembly\01_mag_insertionC.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_mag_insertionD.jpg" data-lity>
        <img src="images\01_assembly\01_mag_insertionD.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
<tr>
    <td> Separate magnet holders and install magnet of opposite polarity to corresponding hole. Tighten snug tight.<br></td>
    <td><B>CAUTION: interference will occur if solder pins are un-clippped!</b>
    </td>
</tr>
<tr>
    <td> <a href="images\01_assembly\01_mag_insertionE.jpg" data-lity>
        <img src="images\01_assembly\01_mag_insertionE.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_mag_insertionF.jpg" data-lity>
        <img src="images\01_assembly\01_mag_insertionF.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
<tr>
    <td> Magnet holder prior to removal with screws snug tight.</td>
    <td>Completed assembly!</b>
    </td>
</tr>
</tbody>
</table>
</div>

Install the remaining magnets and SMD nuts similarly into the open holes of the Probe Board and Tool Board. There might be an interference on the inside edges of the holder and the protruding pins- carefully eject the magnet and tighten the M2 screw. 

### Step 4 - Separate the Boards

Separate the two boards from the PCB rail that joins them by flexing so that they crack between the mousebites holes drilled in the PCBs. If the rail remains attached to one of the boards, it can be carefully removed with flush cutters.

Use a file or nailfile / sandpaper to dress the rear edges of the toolboard. This is the most often offender if the board does not fit into mount recesses. 

<div style="width:100%;text-align:center;">
<table>
<tbody>
<tr>
    <td> <a href="images\01_assembly\01_PCBA.jpg" data-lity>
        <img src="images\01_assembly\01_PCBA.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_PCBB.jpg" data-lity>
        <img src="images\01_assembly\01_PCBB.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
<tr>
    <td> Separate PCB's from rail.</td>
    <td> Clean up mousebites woth file or nailfile. </td>
</tr>
</tbody>
</table>
</div>

### Step 5 – Magnet alignment check:
Place the two boards together and verify that the mating faces are drawn together.
<div style="width:100%;text-align:center;">
 <a href="\images\01_assembly\01_mag_check.jpg" data-lity>
        <img src="images\01_assembly\01_mag_check.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a>
</div>

Grasp the pair of coupled boards between your thumbs and forefingers and try to rock them side to side. If any of the magnet faces are not coplanar, you might feel or hear a slight clicking.

If you believe that this is present, try to identify the pair that is suspect, loosen the fixing screw on one of the magnets, rotate it slightly and re-tighten. This usually takes care of the problem.

### Step 6 - Attach to Mount

Using the provided M2.5 self-tapping screws, or mounting system of your choice, attach the toolbaord PCB to the mount. 
<div style="width:100%;text-align:center;">
<table>
<tbody>
<tr>
    <td> <a href="images\01_assembly\01_mountA.jpg" data-lity>
        <img src="images\01_assembly\01_mountA.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
    <td> <a href="images\01_assembly\01_mountB.jpg" data-lity>
        <img src="images\01_assembly\01_mountB.jpg" style="width:400px; border:2px solid CornflowerBlue">
      </a></td>
</tr>
</tbody>
</table>
</div>
