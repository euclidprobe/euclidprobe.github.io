---
title: "Marlin example macros"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: February 5, 2022
permalink: 06_marlin.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Marlin Probe types and macros
---

Marlin has a few different probe types and probe deploy strategies that can be used, and has built in probe detection.  

The critical part to deciding which probe type to enable will depend on the mechanics and presence of a Z-endstop for the printer. 


### Fixed Mounted Probes
For printers like moving bed / fixed gantry printers, the ```FIXED MOUNTED PROBE``` is one probe option.  Delta printers could also use this this type.  A fixed dock will always be at a fixed Z elevation and therefore no Z movement is needed to deploy or stow the probe. This type of installation would need a custom g-code macro to deploy and stow the probe before use. 

If the Z elevation can be established via an Z-min or Z-max endstop prior to deployment, then a printer that has a bed attached dock and moving Z-gantry could use the same scheme.  

Marlin has a limited set of built in G-code macro variables that could be populated with the required deploy and stow macros that get saved to the SD card and recalled as part of the printer startup. This type of installation would make use of the ```M810 - M819 ```commands. 

Credit to Teaching Tech for reminding us of this method of gcode macros. 

### Allen Key Probes
The one probe type that we have found to work and use the most is the ```ALLEN_KEY_PROBE``` type. While it may be a little more fussy to coordinate and script the dock and stow motions into the ```Configuration.h``` file, it allows the printer to use the native ```M401 / M402``` functionality for things like G29 without having to wrap them between custom gcode macros.  


### Marlin Allen Key Probe Type and Macro Overview
The following is a general outline for deployment and retraction, part of the Configuration.h and Config_adv files (The hardware definition is addressed in the previous section).  Once the deploy and retract strategies are defined, they can be inserted into the firmware, then their execution is automatic on demand. 

The full board setup, probe and Allen Key setup are bundled in the Ender3 config files as example. 

{% include note.html content="Developing the Marlin stepwise deploy and stow strategy is not difficult. The challenge is the tedious nature of writing it into the firmware config file and recompiling.  Users are encouraged to work out the gcode movements as much as they can as a standalone scripts before entering it into the firmware and recompiling." %}

Example gcode script for probe deployment. The coordinates in the Configuration snip below and macros are coordinated to the previous example images. 


### Example deploy.g  

 ```
 G28 X Y              ; home X & Y
 G28 Z                ; Z safe homing
 G0 X100 Y0 Z20 F3000 ; Move to pre-flight - high elevation
 G0 X100 Y0 Z0 F3000  ; Move to pre-flight - low elevation
 G0 X0 Y0 Z0 F1200    ; Move over dock
 G4 P250              ; wait 
 G0 X0 Y40 Z0 F300    ; exit dock
 ``` 

<div style="width:100%;text-align:center;"> <a href="images\06_DeploySteps.png" data-lity> <img src="images\06_DeploySteps.png" style="width:400px; border:2px solid CornflowerBlue"></a></div>


### Example retract.g  

```
G0 X0 Y40 Z20 F300   ; Move ahead of dock - high elevation
G0 X0 Y40 Z00 F300   ; Move ahead of dock - low elevation
G0 X0 Y0 Z0 F1200    ; Enter Dock
G0 X100 Y0 Z0 F3000  ; Swipf by moving right FAST
```

<div style="width:100%;text-align:center;"> <a href="images\06_Retract Steps.png" data-lity> <img src="images\06_Retract Steps.png" style="width:400px; border:2px solid CornflowerBlue"></a></div>


### Configuration.h info

After the above macro scripts successfully execute to deploy and stow the probe, transfer the information to the Configuration.h file section. 



```cpp
/
// For Z_PROBE_ALLEN_KEY see the Delta example configurations.
//
// 
/**
 * Allen key retractable z-probe as seen on many Kossel delta printers - https://reprap.org/wiki/Kossel#Automatic_bed_leveling_probe
 * Deploys by touching z-axis belt. Retracts by pushing the probe down. Uses Z_MIN_PIN.
 */
#define Z_PROBE_ALLEN_KEY

#if ENABLED(Z_PROBE_ALLEN_KEY)
  // 2 or 3 sets of coordinates for deploying and retracting the spring loaded touch probe on G29,
  // if servo actuated touch probe is not defined. Uncomment as appropriate for your printer/probe.
  //
  // DEPLOY STEPS 1- 4 
  //
  #define Z_PROBE_ALLEN_KEY_DEPLOY_1 { 100, 0, 20 }  // Dock side approach position
  #define Z_PROBE_ALLEN_KEY_DEPLOY_1_FEEDRATE XY_PROBE_FEEDRATE

  #define Z_PROBE_ALLEN_KEY_DEPLOY_2 { 100, 0, 0 }  // Drop to dock elevation for probe coupling
  #define Z_PROBE_ALLEN_KEY_DEPLOY_2_FEEDRATE (XY_PROBE_FEEDRATE)/10

  #define Z_PROBE_ALLEN_KEY_DEPLOY_3 { 0, 0, 0 } // Translate over probe in dock 
  #define Z_PROBE_ALLEN_KEY_DEPLOY_3_FEEDRATE XY_PROBE_FEEDRATE

  #define Z_PROBE_ALLEN_KEY_DEPLOY_4 { 0, 40, 0 } // Translate out of dock 
  #define Z_PROBE_ALLEN_KEY_DEPLOY_4_FEEDRATE XY_PROBE_FEEDRATE
  //
  // STOW STEPS 1-4
  //
  #define Z_PROBE_ALLEN_KEY_STOW_1 { 0, 40, 20 } // Move the probe into X,Y dock approach position
  #define Z_PROBE_ALLEN_KEY_STOW_1_FEEDRATE XY_PROBE_FEEDRATE

  #define Z_PROBE_ALLEN_KEY_STOW_2 { 0, 40, 0 } // Move probe down to dock level entry position
  #define Z_PROBE_ALLEN_KEY_STOW_2_FEEDRATE (XY_PROBE_FEEDRATE)/10

  #define Z_PROBE_ALLEN_KEY_STOW_3 { 0, 0, 0 } // Move probe into dock
  #define Z_PROBE_ALLEN_KEY_STOW_3_FEEDRATE XY_PROBE_FEEDRATE

  #define Z_PROBE_ALLEN_KEY_STOW_4 { 100, 0, 0 } // Swipe probe off of mount 
  #define Z_PROBE_ALLEN_KEY_STOW_4_FEEDRATE XY_PROBE_FEEDRATE

#endif // Z_PROBE_ALLEN_KEY
````

