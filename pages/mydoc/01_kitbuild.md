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

## TL:DR 
Open the bag carefully; sort your parts: solder the header and switch; attach your magnets; screw the toolboard to the mount; attach your dock; config your FW; print happily ever after!

## Step 1 – Board Preparation:
The Euclid Probe kit will arrive in a small zip-sealed baggie. Beware, there are small parts that can be easily lost.

The kit contains the PCB set, screws, SMD nuts, a switch, magnets and wiring connectors.

Leave the two PCB’s attached to the rail for now. It will aid in the solder assembly of the components. 

Determine the orientation for the plunger on the switch:
    - Most installations will favor the plunger to the rear of the probe. That way the eccentricity between the nozzle and plunger is minimised. 
    - Installations on printers like Ender3 will benefit from the plunger 

Determine how you will be attaching the upper tool board PCB to your carriage. The mount holes in the upper board are drilled thru 2.5mm⌀:
    - Use the included M2.5x6 self tapping screws into the pilot holes for the provided mounts.
    - Tap pilot holes for with an M3 tap so that you can secure it from above and have concealed fasteners.
    - Drill through with M3mm⌀ and use M3 screws to secure to M3 heatserts embedded in your carraige. This is a popular method. 
    - Countershink for concealed fasteners. There is sufficient material in the PCB to countersink the screw holes to use flat head screws for a flush installation to threaded holes above.
    - The holes are positioned such that if heatserts were used in a carriage, there will be sufficient cover in the margins between the JST connector housing clearance hole and the inserts.

You may want to print out this combined soldering holder & drill-tap guide block that we have designed. It will hold the JST header and switch upright for soldering and as an aid to align an M3 tap or 3mm⌀ drill perpendicular to the toolboard. The differences in versions are the clearance allowances around the outlines. Print the -3 version if you have a reasonably tuned printar.

## Step 2 - Board Assembly:

Install the wiring connector to upper tool board. This PCB has the outline of the JST-XH socket header printed on the backside and has the surface mounted components installed to the front side. Install the connector from the backside of the board so that all the thru-hole soldering will occur on the front side.

Install the switch to the probe board with the footprint labeled SW1. Install the switch from the backside. Note the pin labeling on the PCB silk screen printing. The recommended switch orientation is such that the plunger is oriented towards the blunt end of the board. On most switches, the COM pin is on the side of the plunger. This centers the plunger’s action in line with the fastening screws above and minimizes any eccentric forces on actuation. It is important to fully seat the switch against the PCB when soldering. This eliminates any potential lateral movement of the switch due to bending of the soldered pins, maintaining the best possible probe accuracy.

It is helpful to use a dot of superglue to attach the switch and the connector the board before soldering.
The pre-glued components will aid in keeping the PCB’s inverted and stable for hand soldering without a jig.
The straight male pins may be interchanged with the socket header to use the Dupont style connector.
Solder the switch and connector to the PCB boards.

After soldering you can clip the excess length of the solder pins. 

It is suggested to insulate the exposed terminals of the top side of the probe PCB by placing a piece of Kapton tape (not included) or similar non-conductive material to insulate the exposed terminals. Nail polish or model enamel works well too.

## Step 3 – Magnet Installation
In the kit there are 4, M2x0.4 by 5mm long screws, 4 countersunk magnets and 4 M2 SMD nuts. These are used to secure the magnets to the holders.  

The proper orientation of the magnets is such that the probe will only couple in one specific orientation by opposing the magnet’s polarities. The magnets area ideally orientated so that their poles alternate fore and aft on the board.

We insert the magnets into the shipping holders that identify their polarities and space them the proper distance apart for installation. The intent is that the user only swivels the holders apart to insert the M2 screws thru to install. The magnets will easily eject from the holder in the direction of screw insertion. 

This way, when the tool approaches the probe in the dock, the leading magnet’s polarity is opposite of the first. Since these two magnets are of the same polarity, they are repulsed, pushing the probe into the dock and allowing the tool to pass over. When the tool aligns with the second magnet, the probe will be lifted in the dock and couple with the tool.

Place the shoulder of one of the SMD nuts into one of the holes of the PCB from the same side that the switch was installed from. Push the nut fully into the hole and screw the magnet into the nut. Tighten the screw snug tight. The SMD nut is shallower than the PCB thickness and tightening the screw will cause the magnet to bear against the plated hole, creating the electrical connection. The magnet should now be protruding on the opposite side of the PCB board from the switch.

Install the remaining magnets and SMD nuts similarly into the open holes of the Probe Board and Tool Board. There might be an interefernce on the inside edges of the holder and the protruding pins- carfully eject the magnet and tighten the M2 screw. 

## Step 4 - Seperate the Boards

Separate the two boards from the PCB rail that joins them by flexing so that they crack between the mousebites holes drilled in the PCBs. If the rail remains attached to one of the boards, it can be carefully removed with flush cutters.

Use a file or nailfile / sandpaper to dress the rear edges of the toolboard. This is the most often offender if the board does not fit into mount recesses. 

## Step 5 – Magnet alignment check:
Place the two boards together and verify that the mating faces are drawn together.

Grasp the pair of coupled boards between your thumbs and forefingers and try to rock them side to side. If any of the magnet faces are not coplanar, you might feel or hear a slight clicking.
If you believe that this is present, try to identify the pair that is suspect, loosen the fixing screw on one of the magnets, rotate it slightly and re-tighten. This usually takes care of the problem.