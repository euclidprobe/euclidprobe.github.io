---
title: "Railcore"
keywords: Railcore
tags: [mounts, docks]
last_updated: January 24, 2022
permalink: 02c_Railcore.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Railcore implementation for Euclid Probe
---
Railcore deployment of Euclid Probe is dependent on the hardware choices made at build time. No two Railcores are identical.  The growing convention is to deploy the Euclid dock at Xmin,Ymax and the mount attached to the holes provided for BLTouch.  

The preferred RailCore dock is the 2-part version that mounts to the bottom of the rear extrusion. It is the shortest and therefore the stiffest dock and mount in the offerings. If no extra nuts were placed in the channel, then a number of different options exist:

 - Loosen the belts, remove a corner cube, pop new nuts in the channel and reassemble. It’s a simple yet tedious, 20 minute process. the most direct remedy.
 - Use a rotary tool with a burr to enlarge a section of the extrusion to pass a nut. It is advised that a vacuum be used in conjunction with the rotary tool to prevent chips from migrating into places they shouldnt.
 - Use the provided below drilling jig with either a 6mm or 1/4″ drill bit to spot a hole in the channel. The drill bit is angled 5 degrees to make drill access BEWARE: drilling the edge of the extrusion this way can bind the bit edges and cause strain in the drill. Uses M3 heatserts and M3 screws to expand the ears into the channel. The Print in Place supports should be severed with a hobby/craft knife to release the ears so they can snap into the channel.
 - The other alternative is the clip-on dock mount has been designed to snap onto the back left vertical extrusion and provides for adjustment in X & Y (Z being achieved by sliding the mount up and down). The clamp uses 3-M3X10 screws through the face of the bracket into M3 heatserts set in the back. The L-shaped adjuster and dock attaches to the mount with an M3x12 draw-bolts and nuts. We recommend that the dock get positioned as close as possible to the vertical extrusion.

## Y-Carriage Mounts
The mounts designed for the Standard FDM Y-carriage is the same for the 713Maker Y-carriage plate. 

The mount for the MRW S/D plate is specific to that plate. 

There is a mount specifically designed for the Petsfang fan shroud as well. 

Additionally, through a collaborative effort with 713MAker, there is an all-metal version of the mount and dock for both Stock/713Maker and MRW carriages. 

## Docks
There are 2 types of docks- the 'Corner Clip-On' and the Overhead mount. The corner clip on was designed to try and provide a solution to those who did not install extra nuts in their extrusions. It is limited in its reach. See the screen snips for geometries. 

The Overhead mount attaches to nuts in the bottom slot of the rear extrusion. This is the shortest/stiffest FDM dock.  

713Maker has designed and produces a clever all metal dock that has retrofit T-nuts as well. 


## General Railcore Plan & Dock Offset Dimensions  
<div style="width:100%;text-align:center;">
  <a href="images\02-railcore\02_RC_Corner_Dock.png" data-lity>
  <img src="images\02-railcore\02_RC_Corner_Dock.png" style="width:400px; border:2px solid CornflowerBlue"></a>
  <a href="images\02-railcore\RailCoreTopMount-768x559.jpg" data-lity>  
  <img src="images\02-railcore\RailCoreTopMount-768x559.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
  <a href="images\02-railcore\RailCoreCorner713_YElev.jpg" data-lity>
  <img src="images\02-railcore\RailCoreCorner713_YElev.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
  <a href="images\02-railcore\RailCoreTopMnt713_YElev.jpg" data-lity>
  <img src="images\02-railcore\RailCoreTopMnt713_YElev.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
  <a href="images\02-railcore\RailCoreCornerPlan.jpg" data-lity>
  <img src="images\02-railcore\RailCoreCornerPlan.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
  <a href="images\02-railcore\RailCoreCornerPlan_X_Elev.jpg" data-lity>
  <img src="images\02-railcore\RailCoreCornerPlan_X_Elev.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>

<div style="width:100%;text-align:center;">
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:3px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:3px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:center;vertical-align:middle}
</style>

<table class="tg">
<tbody>
  <tr>
    <td class="tg-0pky">
    <div id="stl_cont0" style="width:450px;height:450px;margin:0 auto;">
      <script>
        var stl_viewer=new StlViewer
        (
          document.getElementById("stl_cont0"), 
          {
              allow_drag_and_drop: false, 
              auto_rotate:true,
              auto_resize:true,
              zoom:110,
              models: 
              [ 
                {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RC_CornerMountV4.5.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
              ]
          }
        );
      </script>
    </div>
    </td>
    <td class="tg-0pky">
    <div id="stl_cont1" style="width:450px;height:450px;margin:5 auto">
      <script>
         var stl_viewer=new StlViewer
         (
           document.getElementById("stl_cont1"), 
           {
               allow_drag_and_drop: false,
               auto_rotate:true,
               auto_resize:true,
               zoom:110,
               models: 
               [ 
                 {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RailCoreTopMountShort.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
               ]
           }
         );
     </script>
    </div> 
    </td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RC_CornerMountV4.5.stl">RailCore Corner Mount</a></td>
    <td class="tg-0pky"><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RC_CornerMountV4.5Dock.stl">RailCore Top Mount</a></td>
  </tr>
  <tr>
    <td class="tg-0pky">
    <div id="stl_cont2" style="width:450px;height:450px;margin:0 auto;">
      <script>
        var stl_viewer=new StlViewer
        (
          document.getElementById("stl_cont2"), 
          {
              allow_drag_and_drop: false, 
              auto_rotate:true,
              auto_resize:true,
              zoom:110,
              models: 
              [ 
                {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RC_CornerMountV4.5Dock.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
              ]
          }
        );
      </script>
    </div>
    </td>
    <td class="tg-0pky">
    <div id="stl_cont3" style="width:450px;height:450px;margin:5 auto">
      <script>
         var stl_viewer=new StlViewer
         (
           document.getElementById("stl_cont3"), 
           {
               allow_drag_and_drop: false,
               auto_rotate:true,
               auto_resize:true,
               zoom:110,
               models: 
               [ 
                 {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RailCoreTopMountDock.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
               ]
           }
         );
     </script>
    </div> 
    </td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RC_CornerMountV4.5.stl">RailCore Corner Mount Dock</a></td>
    <td class="tg-0pky"><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RC_CornerMountV4.5Dock.stl">RailCore Corner Mount Dock</a></td>
  </tr>
</tbody>
</table>
</div>

## Petsfang Dock & Mount Dimensions  
<div style="width:100%;text-align:center;">
  <a href="images\02-railcore\RailCorePetsfang00Image.jpg" data-lity>
  <img src="images\02-railcore\RailCorePetsfang00Image.jpg" style="width:400px; border:2px solid CornflowerBlue"></a>
</div>

<div style="width:100%;text-align:center;">
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:3px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:3px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:center;vertical-align:middle}
</style>
<table class="tg">
<tbody>
<tr>
   <td class="tg-0pky">
     <div id="stl_cont4" style="width:450px;height:450px;margin:5 auto">
        <script>
          var stl_viewer=new StlViewer
          (
          document.getElementById("stl_cont4"), 
            {
                allow_drag_and_drop: false,
                auto_rotate:true,
                auto_resize:true,
                zoom:110,
                models: 
                [ 
                {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RailCorePetsfangMountV1.stl",color:"#1E73BE", rotationx:5.0,    rotationy:-0. 50, rotationz:0.0} 
                ]
            }
          );
        </script>
     </div>
   </td>
   <td>
     <div id="stl_cont5" style="width:450px;height:450px;margin:5 auto">
         <script>
            var stl_viewer=new StlViewer
            (
              document.getElementById("stl_cont5"), 
              {
                  allow_drag_and_drop: false,
                  auto_rotate:true,
                  auto_resize:true,
                  zoom:110,
                  models: 
                  [ 
                    {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RailCorePetsfangMountV2.stl",color:"#1E73BE", rotationx:5.0,    rotationy:-0.50, rotationz:0.0} 
                  ]
              }
            );
        </script>
     </div> 
  </td>
</tr>
<tr>
  <td class="tg-0pky"><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RailCorePetsfangMountV1">RailCore Petsfang Mount V1</a></td>
  <td class="tg-0pky"><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Rail%20Core/RailCorePetsfangMountV2.stl">RailCore Petsfang Mount V2</a></td>
</tr>  
</tbody>
</table>
</div>



