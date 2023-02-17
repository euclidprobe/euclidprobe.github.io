---
title: "Euclid Wiring to Big Tree Tech / BIQU  Hardware"
keywords: probe wiring
tags: [wiring, BTT, BIQU, Octopus, SKR]
last_updated: Feb 5, 2022
permalink: 03_btt.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Euclid Wiring to BTT Hardware
---
### SKR Controller Commissioning
SKR series mainboards can use either the standard 5V or 24V Euclid models. Wire Euclid Probe to any open endstop connector or the Probe connection sockets with some care.    

<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide5.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide5.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR 1.x Series Mainboard Wiring Diagram as Endstop</b></td>
</tr>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide6.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide6.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR 1.x Series Mainboard Wiring Diagram as Probe</b></td>
</tr>
</table>

### SKR Mini Controller Commissioning
SKR Mini series mainboards can use either the standard 5V or 24V Euclid models. Wire Euclid Probe to any open endstop connector or the Probe connection sockets with some care.    
<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide7.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide7.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR Mini Series Mainboard Wiring Diagram as Endstop</b></td>
</tr>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide8.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide8.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR Mini Series Mainboard Wiring Diagram as Probe</b></td>
</tr>
</table>

### SKR Pro Controller Commissioning
SKR Pro mainboards can use either the standard 5V or 24V Euclid models. Wire Euclid Probe to any open endstop connector or the Probe connection sockets with care.    
<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide10.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide10.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR Pro Mainboard Wiring Diagram as Probe</b></td>
</tr>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide9.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide9.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR Pro Mainboard Wiring Diagram as Endstop</b></td>
</tr>
</table>

### SKR 2.0 Controller Commissioning
SKR Pro mainboards can use either the standard 5V or 24V Euclid models. Wire Euclid Probe to any open endstop connector or the Probe connection sockets with care.    
<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide12.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide12.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR 2.0 Mainboard Wiring Diagram as Probe</b></td>
</tr>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide11.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide11.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>SKR Pro Mainboard Wiring Diagram as Endstop</b></td>
</tr>
</table>


### GTR Controller Commissioning
GTR mainboards can use either the standard 5V or 24V Euclid models. Wire Euclid Probe to any open endstop connector or the Probe connection sockets with care.    
<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide13.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide13.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>GTR Mainboard Wiring Diagram as Endstop</b></td>
</tr>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide12.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide12.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>GTR Mainboard Wiring Diagram as Probe</b></td>
</tr>
</table>


### Octopus Commissioning
BTT Octopus has numerous revisions and only one is illustrated below currently. Users are encouraged to verify their deployment needs and coordinate with the schematic and documentation for their specific model. 

Octopus can use either the standard 5V or 24V Euclid models whether Euclid Probe is going to be connected to an open endstop connector or 24V capable probe port. 

If you are using klipper with the Octopus, there are some considerations to make- notably the use of the optocoupled probe port circuit and the BAT85 diode on a remote toolboard. 

If Euclid Probe is to be wired to the Probe Port (pin PB7), you may need to set the probe pin LOW in order for the firmware to recognize the operation (~PB7). See Section 2.7 in the Octopus User Guide under Probe Port Wiring

If Euclid Probe is to be wired to the Endstop Port (pin PG11), you will need to use the BAT85 diode and set the probe pin HIGH in order for the firmware to recognize the operation (^PG11). See Section 2.7 in the Octopus User Guide under Probe Port Wiring

<b>The topic we get the most inquiry about is the opto-coupled probe port on the Octopus.</b> There are seemingly many variations on the optocoupled port. If the LED stays illuminated, then the optocoupler on the controller can not sink enough current for the LEDs to go out. 
<br><b>Our recommendation is to not use the Z_Probe port and use an endstop port instead. </b>

<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide1.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide1.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>Octopus Pro Wiring Diagram with Euclid Probe on Probe Circuit</b></td>
</tr>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide2.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide2.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>Octopus Pro Wiring Diagram with Euclid Probe on Endstop Circuit</b></td>
</tr>
</table>

### Octopus with Remote Toolboard Commissioning
BTT Octopus has numerous revisions and only the Pro is illustrated below currently. Users are encouraged to verify their deployment needs and coordinate with the schematic and documentation for their specific model. 

Octopus can use either the standard 5V or 24V Euclid models whether Euclid Probe is going to be connected to an open endstop connector or 24V capable probe port. 
<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide3.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide3.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>Octopus Pro Wiring Diagram with Euclid Probe connected to remote toolboard on an Endstop Circuit</b></td>
</tr>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide4.PNG" data-lity>
        <img src="images\04-wiring\boards_BTT\Slide4.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
   </td>
</tr>
<tr>
   <td><b>Octopus Pro Wiring Diagram with Euclid Probe connected to remote toolboard on Probe Circuit</b></td>
</tr>
</table>
