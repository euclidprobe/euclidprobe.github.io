---
title: "Comparisons to other Probes"
keywords: probe dock, tool mount
tags: [FAQ]
permalink: 00-others.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Comparing Euclid Probe to other devices
---

### Look at the forums and support channels for yourself ....
Look at the various forums and channels at the help requests for other devices and probes, and the kinds of help requests people put up. The chatter is overwhelmingly about the difficulty in setting up the other popular devices and what happens when they break down or just don't work.  

Now look around and see what kinds of requests are out there for Euclid Probe. There are not that many! Euclid is as simple and efficient as a probe can get. The most often raised concern is how to customize the macros or tweaking a mount or dock. There are an overwhelming number of comments from users who essentially say the same thing:<b> "Bolt it on, configure your firmware, print happily ever after"</b>  

### Don't take our word for it, look at what the competition says .... 
The original data in the following table was originally published at BLTouch's website.
  <a href="images\00-BLTouch.png" data-lity>
    <img src="images\00-BLTouch.png" style="width:50px; border:2px solid CornflowerBlue"></a>  

 We've added a couple of rows and columns to fill in the missing data...  
 TH3D does not publish and data for EZABL. 

<div style="width:100%;text-align:center;">
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-vfn0{background-color:#efefef;border-color:#000000;text-align:center;vertical-align:top}
.tg .tg-g5f9{background-color:#3166ff;border-color:#000000;color:#ffffff;text-align:center;vertical-align:top}
.tg .tg-73oq{border-color:#000000;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-g5f9">Sensor</th>
    <th class="tg-g5f9">BLTouch<br> (Hall)</th>
    <th class="tg-g5f9">Proximity<br>Inductive</th>
    <th class="tg-g5f9">Proximty<br>Optical</th>
    <th class="tg-g5f9">Micro Switch<br> with SG90 Servo</th>
    <th class="tg-g5f9">EZABL</th>
    <th class="tg-g5f9">Euclid Probe</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-73oq">Sensor Type</td>
    <td class="tg-73oq">contact</td>
    <td class="tg-73oq">non-contact</td>
    <td class="tg-73oq">non-conact</td>
    <td class="tg-73oq">contact</td>
    <td class="tg-73oq">non-contact</td>
    <td class="tg-73oq">contact</td>    
  </tr>
  <tr>
    <td class="tg-vfn0">Standard Deviation</td>
    <td class="tg-vfn0">&le;0.01</td>
    <td class="tg-vfn0">&le;0.2</td>
    <td class="tg-vfn0">&le;0.01</td>
    <td class="tg-vfn0">&le;0.3</td>
    <td class="tg-vfn0">?</td>
    <td class="tg-vfn0">&le;0.0015</td>
  </tr>
  <tr>
    <td class="tg-73oq">Repeated Accuracy</td>
    <td class="tg-73oq">&le;1%</td>
    <td class="tg-73oq">&le;5%</td>
    <td class="tg-73oq">&le;1%</td>
    <td class="tg-73oq">&le;5%</td>
    <td class="tg-73oq">?</td>
    <td class="tg-73oq">&le;0.2%</td>
  </tr>
  <tr>
    <td class="tg-vfn0">Bed Material</td>
    <td class="tg-vfn0">Unlimited</td>
    <td class="tg-vfn0">Metallic</td>
    <td class="tg-vfn0">Glass X</td>
    <td class="tg-vfn0">Unlimited</td>
    <td class="tg-vfn0">?</td>
    <td class="tg-vfn0">Unlimited</td>
  </tr>
  <tr>
    <td class="tg-73oq">Max Current</td>
    <td class="tg-73oq">&le;300mA</td>
    <td class="tg-73oq">&le;200mA</td>
    <td class="tg-73oq">&le;2300mA</td>
    <td class="tg-73oq">&le;300mA</td>
    <td class="tg-73oq">?</td>
    <td class="tg-73oq">6mA</td>
  </tr>
  <tr>
    <td class="tg-vfn0">Current Consumption</td>
    <td class="tg-vfn0">20mA</td>
    <td class="tg-vfn0">20mA</td>
    <td class="tg-vfn0">20mA</td>
    <td class="tg-vfn0">200mA w/t jitter<br>20mA w/o jitter</td>
    <td class="tg-vfn0">?</td>
    <td class="tg-vfn0">6mA when deployed<br>0mA when docked</td>
  </tr>
  <tr>
    <td class="tg-73oq">Affected by Bed Heat</td>
    <td class="tg-73oq"><b><span style="color:red">&#10004;</span></b></td>
    <td class="tg-73oq"><b><span style="color:red">&#10004;</span></b></td>
    <td class="tg-73oq">?</td>
    <td class="tg-73oq">?</td>
    <td class="tg-73oq">?</td>
    <td class="tg-73oq"><b><span style="color:green">NO</span></b></td>
  </tr>
   <tr>
    <td class="tg-vfn0">Affected by Magnetism</td>
    <td class="tg-vfn0"><b><span style="color:red"> &#10004;</span></b> </td>
    <td class="tg-vfn0"><b><span style="color:red">&#10004;</span></b> </td>
    <td class="tg-vfn0"></td>
    <td class="tg-vfn0"></td>
    <td class="tg-vfn0">?</td>
    <td class="tg-vfn0"><b><span style="color:green">NO</span></b></td>
  </tr>
  <tr>
    <td class="tg-73oq">Notes:</td>
    <td class="tg-73oq">Proprietary cable with Molex Picoblade</td>
    <td class="tg-73oq">Accuracy of NPN and PNP type sensors vary widely by manuf'r</td>
    <td class="tg-73oq"></td>
    <td class="tg-73oq"></td>
    <td class="tg-73oq">Requires external controller module and external 12V power supply</td>
    <td class="tg-73oq"><b><span style="color:green">24V Input capable</span></b></td>
  </tr>
     <tr>
    <td class="tg-vfn0">Cost (not including shipping</td>
    <td class="tg-vfn0">&ge;$40USD</td>
    <td class="tg-vfn0">&ge;$15USD</td>
    <td class="tg-vfn0">&ge;$25USD</td>
    <td class="tg-vfn0">&ge;$10USD</td>
    <td class="tg-vfn0">&ge;$65USD</td>
    <td class="tg-vfn0">$25USD</td>
  </tr>
</tbody>
</table>
</div>
(BTLtouch is a registered product of ANTCLABS, Republic of Korea. EZABL&#8482; trademarked by TH3DStudio.) 
