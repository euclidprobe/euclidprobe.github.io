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
Currently there are 2 versions of Euclid Probe kits available. There is now difference in price. 

The standard version was developed to use the controller's logic voltage to illuminate the LED's. Generally speaking, 16bit boards used 5V and 32bit boards used 3.3V.  All Euclid Probe versions will work with these controllers. Example controllers include MEGA/RAMPS, Duet3d controllers, 32bit LPC based controllers like Smoothieboard, SKR1.4, MKS Base, etc...  

With the development of the high voltage capable controllers that use a remote toolboard, we developed a version of Euclid Probe that will work with all voltages including 24V voltage provided by these toolboards to power the LED's and return the signal via the wiring bundle to the controller. Do not directly wire a regular 5V Euclid to 24V, it will most likely burn out the LEDs and resistors. 

The 24V capable PROBE ports on the various controllers are not standard or uniform. While we do our best to try and provide users all the necessary documentation as we encounter the various controllers.  Users should expect to coordinate the wiring of Euclid Probe to their controller and their firmware configuration. 

{% include tip.html content="24V Euclid version works with all voltages." %}

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
</table>
</div>
