---
title: "Voron Trident"
keywords: probe dock, tool mount
tags: [mounts, docks]
last_updated: Feb 5, 2022
permalink: 02c_VoronTrident.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Voron Trident Probe Docks & Mount 
---

## Gantry Mounted Voron Trident Dock
The Voron Trident mounts were collaboratively developed with Trident users to be located at the left-rear motor mount.  Version 2 is the most current- we leave Version 1 here as well for reference. The toolboard can be mounted to either the native carriage or to the standard Omron adapter. 

### Gantry Mount Version 1 & 1.1
Gantry mount Version 1.1 utilizes M5x16 and M5x30 screws from the BOM to attach through the left side motor mount bracket into the extrusion.  The 1.1 mirrored version provides clearance to the motor wiring if present.  

<b> Version 1.1 mirrored is the currently preferred gantry mounted dock and dock mount. </b>

Vertical adjustment of the dock is done by loosening the hidden M5x16 thru-bolt screw via the keyhole in the front of the dock and raising/lowering the dock vertically with the keyed slot.  The M5 nut is captured in the keyhole/slot in the dock mount. 

<div style="width:100%;text-align:center;">
<a href="images\02-voron\VoronGantryMountRev1.1Mirrored.jpg" data-lity>
<img src="images\02-voron\VoronGantryMountRev1.1Mirrored.jpg" style="height:250px; border:2px solid CornflowerBlue"></a>
<a href="images\02-voron\VoronGantryMountRev1.1Mirrored2.jpg" data-lity>
<img src="images\02-voron\VoronGantryMountRev1.1Mirrored2.jpg" style="height:250px; border:2px solid CornflowerBlue"></a>
<a href="images\02-voron\Trident_TopMountXRay2.png" data-lity>
<img src="images\02-voron\Trident_TopMountXRay2.png" style="height:250px; border:2px solid CornflowerBlue"></a>
</div>

<div style="width:100%;text-align:center;">
<table>
  <tr>
    <td>
    <div id="stl_cont00" style="width:450px;height:450px;margin:0 auto;">
      <script>
        var stl_viewer=new StlViewer
        (
          document.getElementById("stl_cont00"), 
          {
              allow_drag_and_drop: false, 
              auto_rotate:true,
              auto_resize:true,
              zoom:110,
              models: 
              [ 
                {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/Trident_TopMountCloseV1.1Mirrored.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
              ]
          }
        );
      </script>
    </div>
    </td>
    <td>
    <div id="stl_cont01" style="width:450px;height:450px;margin:5 auto">
      <script>
         var stl_viewer=new StlViewer
         (
           document.getElementById("stl_cont01"), 
           {
               allow_drag_and_drop: false,
               auto_rotate:true,
               auto_resize:true,
               zoom:110,
               models: 
               [ 
                 {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/Trident_TopMountDockCloseV1.1Mirrored.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
               ]
           }
         );
     </script>
    </div> 
    </td>
  </tr>

  <tr>
    <td ><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/Trident_TopMountCloseV1.1Mirrored.stl">Voron Trident Dock Mount Version 1.1 Mirrored </a></td>
    <td ><a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/Trident_TopMountDockCloseV1.1Mirrored.stl">Voron Trident Dock Version 1.1 Mirrored </a></td>
  </tr>
</table>
</div>  

Version 1 utilized non-BOM fasteners for attachment. We leave Version 1 in the archive for convenience.  
<div style="width:100%;text-align:center;">
<a href="images\02-voron\Trident_TopMount.png" data-lity>
<img src="images\02-voron\Trident_TopMount.png" style="height:250px; border:2px solid CornflowerBlue"></a>  
</div>  

### Gantry Mount Version 2(Revision 4)
Version 2 of the gantry mount is fixed in height and location. This mount is intended to utilize the Omron adapter to fine tune the height of the probe into the dock.  

Version 2 SHORT of the gantry mount is fixed in height and location and is for users of the native carriage shells.It requires the use of shims to provide fine tuning of the probe height. Users are cautioned that this is not a straightforward plug-and-play installation.  

A recess for either a magnet or M3 nut has been provided in the nose of the dock to server as a keeper for the probe.  

This mount attaches through and clamps the left side motor mount bracket with an M5x16 and M5x30 screw from the BOM. Two small shear lug rings are provided to key the dock to the motor mount- if the print quality of the two parts is not the greatest, they might interfere and removal is recommended.  This was developed with the collaboration of Discord users Dattas, Deepsiks and Kyleisah.


<div style="width:100%;text-align:center;">

<a href="images\02-voron\VoronGantryMountRev2.jpg" data-lity>
<img src="images\02-voron\VoronGantryMountRev2.jpg" style="height:250px; border:2px solid CornflowerBlue"></a>
</div>  

<div style="width:100%;text-align:center;">
<table>
<tr>
<td>
<div id="stl_cont02" style="width:450px;height:450px;margin:0 auto;">
  <script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont02"), 
      {
          allow_drag_and_drop: false, 
          auto_rotate:true,
          auto_resize:true,
          zoom:200,
          models: 
          [ 
            {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev_4_Set.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
  </script>
</div>  
</td>
<td>
<div id="stl_cont03" style="width:450px;height:450px;margin:0 auto;">
  <script>
    var stl_viewer=new StlViewer
    (
      document.getElementById("stl_cont03"), 
      {
          allow_drag_and_drop: false, 
          auto_rotate:true,
          auto_resize:true,
          zoom:200,
          models: 
          [ 
            {filename:"https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev2_Short.stl",color:"#1E73BE", rotationx:5.0, rotationy:-0.50, rotationz:0.0} 
          ]
      }
    );
  </script>
</div>  
</td>
</tr>
<tr>
<td>
  <a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev_4_Set.stl" target="blank">Voron 2.4 and Trident Gantry Mount Version 2Rev4</a>  
  </td>
  <td>
  <a href="https://raw.githubusercontent.com/nionio6915/Euclid_Probe/main/stls/Voron/VoronGantryMountRev2_Short.stl" target="blank">Voron 2.4 and Trident Gantry Mount Version 2Rev4 Short</a>  
  </td>
  </tr>
  </table>  
  </div>  

## CAD Files
The current CAD files are <a href='https://github.com/nionio6915/Euclid_Probe/tree/main/CAD' target="_blank"><b> available here in the repo.</b></a>
