---
title: "Wiring the Tool Board"
keywords: probe wiring
tags: [wiring]
last_updated: Feb 5, 2022
permalink: 03_wiring.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Electrical Requirements - Wiring the Tool Board
---

Febraury 5, 2022: We are updating page maintenance and updating product images. Each of the controller pages will be a little sparse as we progress. 

### Commisioning
The first step in commissioning Euclid Probe is deciding if the device will be wired as a Z-Probe or an endstop. Euclid Probe can be configured in most printer firmwares as both and endstop and as a probe.  

Refer to your printers firmware documentation for determining the most ideal way for your configuration.

{% include tip.html content="The most direct method of wiring Euclid Probe is connecting it to an unused endstop connector." %} 

Wiring to other ports such as dedicated Z-probe or remote I/O ports are also possible. 

### 5V & 24V Version Differences 
Euclid Probe can be wired direct to a remote toolboard that provides 24V sensing voltage and used with a controller that has a 24V probe input. In this application, the 24V version is most appropriate. The 24V version is all voltage capable.  

If your controller is not high voltage capable, the the standard 5V model is sufficient.  This includes RAMPS based controllers, Duet2 and Duet3 hardware, most LPC and STM based controllers without high voltage inputs. 

{% include warning.html content="If a 5V model is connected to 24V at the VCC pin, the LED's and resistors can not tolerate the higher current and will likely burn up" %} 

{% include tip.html content="After soldering, clip the protruding solder pins flush and cover the exposed solder joints with a bit of tape or paint with nailpolish to insulate. This keeps the blue magic smoke genie in the bottle" %}

### Basic Wiring: 2-wire mode
The Euclid Probe can be wired and function with as few as 2 wires connecting the SIG & GND pins on the toolboard to the controller. The LED’s will not illuminate in 2-wire mode.

<div style="width:100%;text-align:center;">
 <a href="images\04_2wire_example.jpg" data-lity>
        <img src="images\04_2wire_example.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>

Using the appropriate wiring crimps and connector shells, terminate the wiring of your choice and connect the wiring loom to your controller.

Perform a function check with a multimeter or test light before final installation of Euclid Probe.  With the probe and toolboard coupled, use the Continuity Function of your meter and check for continuity across the pins marked GND & SIG. If the circuit is complete, the probe was assembled and coupled correctly.

### Intermediate wiring: LED operation, 3-wire mode
To illuminate the LED’s on the toolboard, a third wire must be connected to the VCC pin on the tool board. This wire should be connected to the logic voltage of he controller, the same way as with 3-wire endstops with LED's. 

{% include important.html content="LED function: the LED's illuminate when the probe is successfully connected to the toolboard.  
Depressing the switch will cause the circuit to open and the LED's to turn off.  
The LED's will blink off when the machine is probing the bed." %} 

<div style="width:100%;text-align:center;">
 <a href="images\04_3wire_example.jpg" data-lity>
        <img src="images\04_3wire_example.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>  
<p></p>

Early Euclid boards and current DIY boards have a connector pinout that is ordred GND-SIG-VCC. If a pre-terminated endstop cable is used to connect Euclid to the controller, two of the terminals will likely need to be re-pinned. 

Current Euclid Probe kits have, and future DIY boards will have, the more conventional SIG-GND-VCC pin order and can be connected with a premade straight through endstop cable.  

### Replacing a BLTouch / CR Touch device
Some controllers have a dedicated 5-pin connecters for these devices. Two of these pins are dedicated to the SIG-GND function of the device as I/O and the other 3-pins are dedicated to the operation of the internal mechanical devices as servo devices. 

The probe signal pin may or may not be 5V tolerant. It is recommended to verify your controller's requirements and if in doubt, use an unused endstop connector instead. 
<div style="width:100%;text-align:center;">
 <a href="images\04_BLT_example.jpg" data-lity>
        <img src="images\04_BLT_example.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>  
<p></p>

### Advanced Wiring
Wiring Euclid Probe to a remote toolboard requires coordination with the controller manual and related device schematics. 
 - Early high-voltage boards made use of a BAT85 diode which acted as a current limiter on the probe circuit. 
 - Some toolhead boards require removal of the remote BAT85 Diode for proper operation of optocouplers on the controller.   
 - CAN type controllers can provide 3.3V or 5v on their I/O ports. 

<div style="width:100%;text-align:center;">
 <a href="images\04_CANB_example.jpg" data-lity>
        <img src="images\04_CANB_example.jpg" style="width:250px; border:2px solid CornflowerBlue"></a>
 <a href="images\04_24VTB_example.jpg" data-lity>
        <img src="images\04_24VTB_example.jpg" style="width:250px; border:2px solid CornflowerBlue"></a>
</div>  
<p></p>