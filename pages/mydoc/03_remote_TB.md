---
title: "CAN Boards & Remote Tool Head boards"
keywords: probe wiring toolhead CAN remote SHT-36 EBB-36
tags: [CAN BUS]
last_updated: October 24, 2022
permalink: 03_remote_TB.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: CAN bus boards,  Wiring the Tool Board
---
# Commissioning
Wiring Euclid Probe to a remote toolboard requires coordination with the controller manual and related device schematics. 
{% include tip.html content="The most direct method of wiring Euclid Probe is connecting it to an endstop connector." %}  
 - CAN type controllers can provide 3.3V or 5v on their I/O ports. Look to use an endstop port. 
 - Early high-voltage break-out boards made use of a BAT85 diode which acted as a current limiter on the probe circuit. Depending on the wiring method, you may or may not need that diode. 
 - Some controllers utilize an optocouplers on the controller.  Not all optocouplers can sink enough current to illuminate / turn off the Euclid LED's.   
<br>

# Huvud CAN BUS Boards
The HUVUD toolboard is designed to simplify wiring and configuration for extruders on klipper-based machines, particularily useful for toolchangers or extra large machines, but provides advantages for even the smallest of machines. Huvud's can be found at resellers like LukesLabonline.com and Fabreeko.com.  
<br>
<div style="width:100%;text-align:center;">
 <a href="images\04_CANB_example.jpg" data-lity>
        <img src="images\04_CANB_example.jpg" style="width:350px; border:2px solid CornflowerBlue"></a>
</div>  

# Duet3 Toolboard 
Wire Euclid Probe to the Probe port any open endstop or I/o connector.  
## Duet3 LC1 Toolboard Wiring Diagram  
<div style="width:100%;text-align:center;">
<a href="images\04-wiring\boards_Duet\Slide5.PNG" data-lity>
          <img src="images\04-wiring\boards_Duet\Slide5.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
</div>  

## Duet3 LC1 Toolboard Wiring as Picture  

<div style="width:100%;text-align:center;">
<a href="images\04-wiring\boards_Duet\Slide6.PNG" data-lity>
<img src="images\04-wiring\boards_Duet\Slide6.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
</div>  


# FLY Mellow CAN BUS Boards
## SB-2040 
<div style="width:100%;text-align:center;">
 <a href="images\03\Slide16.PNG" data-lity>
<img src="images\03\Slide16.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
</div>  <br>  

## FLY-SHT36  
<div style="width:100%;text-align:center;">        
 <a href="images\03\Slide12.PNG" data-lity><br>
        <img src="images\03\Slide12.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
</div>  <br>

## FLY-SHT42  
<div style="width:100%;text-align:center;">
<a href="images\03\Slide13.PNG" data-lity><br>
        <img src="images\03\Slide13.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>     
</div>  <br>

# BTT CAN BUS Boards

## BTT EBB36    
<div style="width:100%;text-align:center;">
 <a href="images\03\Slide14.PNG" data-lity>
        <img src="images\03\Slide14.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
</div>  <br>

## BTT EBB42    
<div style="width:100%;text-align:center;">
 <a href="images\03\Slide15.PNG" data-lity>
        <img src="images\03\Slide15.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
</div>  <br>
