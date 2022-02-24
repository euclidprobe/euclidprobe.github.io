---
title: "Euclid Wiring to Duet3 Hardware"
keywords: probe wiring
tags: [wiring, Duet3]
last_updated: Feb 5, 2022
permalink: 03_duet3.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true  
summary: Euclid Wiring to Duet3 Hardware
---

### Duet3 6HC Mainboard Commissioning
Duet3 mainboard can use either the standard 5V or 24V Euclid models. Wire Euclid Probe to the Probe port any open endstop connector.  

<table>
 <tr>
     <td> <a href="images\04-wiring\boards_Duet\Slide2.PNG" data-lity>
         <img src="images\04-wiring\boards_Duet\Slide2.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
     </td>
 </tr>
 <tr>
     <td><b>Duet3 Mainboard Wiring Diagram</b>
     </td>
 </tr>

 <tr>
     <td> <a href="images\04-wiring\boards_Duet\Slide1.PNG" data-lity>
         <img src="images\04-wiring\boards_Duet\Slide1.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
     </td>
 </tr>
 <tr>
     <td><b>Duet3 Mainboard Wiring as Picture</b>
     </td>
 </tr>
 </table>  
<br> 

### Duet3 3HC Expansions Board
At this time, we do not recommend connecting Euclid to any I/O inputs on the 3HC expansion. There was limitation early in the development of RRF3 with motors and probes/endstops being on different boards. We have not verified that the limitation of motors and endstops/probes being on different boards have been resolved. 


### Duet3 Toolboard Commissioning
Duet3 mainboard and toolboards can use either the standard 5V or 24V Euclid models. Wire Euclid Probe to the Probe port any open endstop connector.    

<table>
 <tr>
     <td> <a href="images\04-wiring\boards_Duet\Slide5.PNG" data-lity>
          <img src="images\04-wiring\boards_Duet\Slide5.PNG" style="width:350px; border:2px solid CornflowerBlue"></a></td>
 </tr>
 <tr>
     <td><b>Duet3 LC1 Toolboard Wiring Diagram</b>
     </td>
 </tr>
 <tr>
     <td> <a href="images\04-wiring\boards_Duet\Slide6.PNG" data-lity>
         <img src="images\04-wiring\boards_Duet\Slide6.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
     </td>
 <tr>
     <td><b>Duet3 LC1 Toolboard Wiring as Picture</b>
     </td>
 </tr>
</table>