---
title: "Euclid Probe Accuracy"
keywords: probe dock, tool mount
tags: [FAQ]
permalink: 00-accuracy.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Background 
---
### Probe Accuracy Testing

Little to no application data was available for the types of switches used in Euclid Probe. Therefore, the engineers and designers who created Euclid Probe embarked on their own testing campaign to qualify the switches and the other components used in construction. This includes mechanical accuracy testing of the individual switches, the entire probe assembly, and actual probe deployment and probe docking cycles on our test printers.

To date, over 500,00 probe deploy-probe-retract cycles with a moving Z-axis dock have been performed. The only probe docking failures were due to operator error: not updating the probe Z-offset between sample changes.

The gathered data was compiled and analyzed to compare the performance between different switch manufactures and models. The overall results have been quite revealing- the usual suspects are not as accurate as they are purported to be, and the other brands and models often dismissed are actually quite accurate.  

Repeatabilities often approach 0.001mm.  

Here is an example of a single switch’s probing results performed at room temperature. Note the trends of the blue vertical bars showing the trigger point in the speed ranges noted at the top.   

Also not the population of the probe points in relationship to the standard of deviation bars noted in orange. The standard of deviation bars are for the total population.

<div style="width:100%;text-align:center;">
  <a href="images\00-ProbeTest57_19_45-768x559.png" data-lity>
    <img src="images\00-ProbeTest57_19_45-768x559.png" style="width:300px; border:2px solid CornflowerBlue">
  </a>
  <p><span style="color:blue">Click image to enlarge</span>.</p>
  
</div>

### How accurate is Euclid Probe? 
Generally speaking, an order of magnitude more accurate than the nearest competing devices or technologies. 

The probing results will vary based on the firmware and mechanical system of the printer, but we have seen repeatabilities  approaching 0.0005mm.  

Below is a bed map submitted by a user who was convinced that Euclid Probe was being influenced by the bed magnets. Note that the Z variation is inverted (what is 'low' is actually being displayed 'hi').


After some consulting with the user, we advised them to place paper shims over the magnets to determine if there was a hollow over the top of the magnet which would draw down the steel build plate. The results were that the steel build surface was truly being drawn into the hollow above the recessed magnets. The user the carefully shimmed each magnet with paper and cigarette rolling paper shims to level the bed.  This was their result- 

<div style="width:100%;text-align:center;">
  <a href="images\00-accuracyA.png" data-lity>
    <img src="images\00-accuracyA.png" style="width:300px; border:2px solid CornflowerBlue">
      <p><span style="color:blue">Click image to enlarge</span>.</p>
  </a>

  <a href="images\00-accuracy-fixed.png" data-lity>
    <img src="images\00-accuracy-fixed.png" style="width:300px; border:2px solid CornflowerBlue">
      <p><span style="color:blue">Click image to enlarge</span>.</p>
  </a>
</div>


### No, really its that good! 
Here is actual output from a user who is using a Euclid Probe on a Railcore 300ZL printer- 2 iterations of their bed tilt adjustment macro- 

```
23:08:32  // probe at 10.000,10.000 is z=9.526562
23:08:33  // probe at 10.000,10.000 is z=9.530000
23:08:34  // probe at 10.000,10.000 is z=9.529375
23:08:36  // probe at 295.000,116.000 is z=9.431875
23:08:37  // probe at 295.000,116.000 is z=9.430937
23:08:38  // probe at 295.000,116.000 is z=9.430937
23:08:40  // probe at 10.000,239.000 is z=9.483750
23:08:41  // probe at 10.000,239.000 is z=9.482812
23:08:42  // probe at 10.000,239.000 is z=9.482812
23:08:42  // Making the following Z adjustments:
// stepper_z = 0.119567
// stepper_z1 = 0.069290
// stepper_z2 = 0.004405
23:08:42  // Retries: 0/4 Probed points range: 0.097396 tolerance: 0.005000
23:08:43  // probe at 10.000,10.000 is z=9.419345
23:08:44  // probe at 10.000,10.000 is z=9.419657
23:08:45  // probe at 10.000,10.000 is z=9.419032
23:08:47  // probe at 295.000,116.000 is z=9.417470
23:08:48  // probe at 295.000,116.000 is z=9.417470
23:08:49  // probe at 295.000,116.000 is z=9.417157
23:08:51  // probe at 10.000,239.000 is z=9.419970
23:08:52  // probe at 10.000,239.000 is z=9.419657
23:08:53  // probe at 10.000,239.000 is z=9.419345
23:08:53  // Making the following Z adjustments:
// stepper_z = -0.000527
// stepper_z1 = -0.000184
// stepper_z2 = -0.002831
23:08:53  // Retries: 1/4 Probed points range: 0.002292 tolerance: 0.005000
23:08:53  // Docking Euclid probe
```

### Don't take our word for it, look at what the competition says .... 
The original data for the following table was published at BLTouch's website.
  <a href="images\00-BLTouch.png" data-lity>
    <img src="images\00-BLTouch.png" style="width:50px; border:2px solid CornflowerBlue"></a>  

 We've added a couple of row and columns to fill in some missing data...  
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
