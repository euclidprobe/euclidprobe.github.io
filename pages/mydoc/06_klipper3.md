---
title: "klipper example Macros"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: February 5, 2022
permalink: 06_klipper3.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: klipper Macros
---

### klipper Macro examples
Due to the organic and idiomatic nature of klipper, there is no standard method to deploy and retract a probe. Therefore, we offer a basic set of macros which serve as a framework for users to customize. The following macros are fundamental and will hopefully get one printing upon commissioning. 

{% include tip.html content="In the following example we maintain the use of M401 and M402 for probe deploy and retract for gcode consistency. Users are encouraged to modify the code to suit their needs." %}

User contributed macros for various printers and configurations are shared in the klipper folder as well. These are offered as a convenience only and are thus unsupported. 

The main example given is for a fixed dock (X, Y, Z constant), with a Z endstop,  with a few example macros. 

If a series of probing commands is desired, then it is recommended that and M401 and M402 pair bracket the sequence of gcodes. See the macro examples homez.g and bed4point.g macros for recommendations.  

{% include warning.html content="When implementing 3rd party macros, pay particular attention to any variables that reference things like Z-Travel height or Z moves after probing or probe pickup.<br>
We recommend a Z-move or travel height of 15mm to ensure that there is enough clearance between the probe and bed." %}

{% include tip.html content="The most up-to-date macros are in the github repository as a bundled .zip file for download - [Euclid github repo](https://github.com/nionio6915/Euclid_Probe/tree/main/Firmware_Examples/klipper)" %}

{% include note.html content="klipper macro syntax does not play well with jekyll\Liquid. The below macro example is presented as an image of the machine code.  The following imost up-to-date macros are in the github repository - [Euclid klipper github repo](https://github.com/nionio6915/Euclid_Probe/tree/main/Firmware_Examples/klipper)" %}

<div style="width:100%;text-align:center;">
 <a href="https://github.com/nionio6915/Euclid_Probe/blob/main/Firmware_Examples/Klipper/00-euclid_exampleV3.cfg">
        <img src="images\06-klipper3.png" style="width:800px; border:2px solid CornflowerBlue"></a>
</div>  
