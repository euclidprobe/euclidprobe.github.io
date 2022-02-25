---
title: "Euclid Probe Voltages"
keywords: probe, version, voltage
tags: [FAQ]
permalink: 00-voltage.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: What is the difference in voltage versions? 
---
### Different Voltage Versions
Currently there are 2 versions of Euclid Probe kits available. There is no difference in price. The voltage only matters if you intend to illuminate the LEDs as status and function indicators. 

The 5V standard version was developed to use a normal endstop port and endstop cable to the controller, and the VCC logic voltage to illuminate the LED's. This is the more universal application. Logic voltage will likely never become more that 3.3V or 5V.

The 24V version was developed to wire natively to the provided probe port on the remote toolboards that can not provide logic voltage onboard.  

#### Are you deploying to an endstop port? 
<div style="width:100%">
<center>
<table>
<tr>
   <td> <a href="images\04-wiring\boards_BTT\Slide5.PNG" data-lity>
<img src="images\04-wiring\boards_BTT\Slide5.PNG" style="width:350px; border:2px solid CornflowerBlue"></a>
  </td>
</tr>  
<tr>
  <td>
   <b>Then all you need is the 5V version</b>
  </td>
</tr>
</table>
</center>
</div>

#### Are you using a remote CAB-BUS controller?  
<div style="width:100%">
<center>
<table>
<tr>
   <td> <a href="images\04_CANB_example.jpg" data-lity>
        <img src="images\04_CANB_example.jpg" style="width:250px; border:2px solid CornflowerBlue"></a>
  </td>
</tr>  
<tr>
  <td>
   <b>Then all you need is the 5V version</b>
  </td>
</tr>
</table>
</center> 
</div>

#### Are you using a remote toolboard? 
<div style="width:100%">
<center>
<table>
<tr>
   <td><a href="images\04-wiring\boards_BTT\Slide4.PNG" data-lity>
       <img src="images\04-wiring\boards_BTT\Slide4.PNG" style="width:400px; border:2px solid CornflowerBlue"></a>  
    </td>
</tr>  
<tr>
  <td>
   <b>Then all you need is the 24V version</b>
  </td>
</tr>
</table>
</center> 
</div>

### Logic Voltages
Generally speaking, 16bit boards used 5V logic and 32bit boards used 3.3V logic. Example 16bit controllers include MEGA/RAMPS. AM based Duet3d controllers, LPC based controllers like Smoothieboard, SKR1.4, MKS Base, etc... All Euclid Probe versions will work with these controllers when plugged into a normal endstop port. 

The 24V capable PROBE ports on the various controllers are not standard or uniform. While we do our best to try and provide users all the necessary documentation as we encounter the various controllers.  Users should expect to coordinate the wiring of Euclid Probe to their controller and their firmware configuration. 

As always, if you need assistance or have questions, please feel free to contact us via the Feedback link above of via the Discord channel. 

<div style="width:100%;text-align:center;">
<table>
<tr>
  <td>  <a href="images\01_5VPCB.jpg" data-lity>
    <img src="images\01_5VPCB.jpg" style="width:400px; border:2px solid CornflowerBlue">
  </a>
  </td>
  <td>
    <a href="images\01_24VPCB.jpg" data-lity>
    <img src="images\01_24VPCB.jpg" style="width:400px; border:2px solid CornflowerBlue">
  </a>
  </td>
</tr>
<tr>
  <td>5V Version</td>
  <td>24V Version</td>
</tr>
<tr>
  <td>Note the absence of 24V markings<P>  
      Note the size and orientation of SMT components</p></td>
  <td>Note the 24V markings on the PCB<P>  
      Note the size and orientation of SMT components</p></td>
</tr>
<tr>
  <td><span style="color:blue">Click images to enlarge</span>
  </td>
  <td><span style="color:blue">Click images to enlarge</span>
  </td>
</tr>
<tr>
  <td>
    <a href="https://tinyurl.com/yawtohnf" data-lity>
    <img src="images\00-falstad.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
  </td>
  <td>
    <a href="https://tinyurl.com/y9l7q26f" data-lity>
    <img src="images\00-falstad.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
  </td>    
</tr>
<tr>
  <td>Euclid as typical 3.3V/5V endstop or Z-Probe input simulation<p>
  <span style="color:blue">Click images to enlarge and simulate</span></p></td>
  <td>Euclid as 24V Z-Probe input simulation<p>
  <span style="color:blue">Click images to enlarge and simulate</span></p></td>
</tr>
</table>
</div>