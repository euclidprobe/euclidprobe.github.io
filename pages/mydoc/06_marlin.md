---
title: "Marlin example macros"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: February 5, 2022
permalink: 06_marlin.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Marlin Macros
---

### Marlin Macro Overview

Marlin configuration is highly dependent on the controller board used. The following is a general outline for deployment and retraction, part of the Configuration.h and Config_adv files (The hardware definition is addressed in the previous section).  

```cpp
//===========================================================================
//============================== Endstop Settings ===========================
//===========================================================================
// @section homing

// Specify here all the endstop connectors that are connected to any endstop or probe.
// Almost all printers will be using one per axis. Probes will use one or more of the
// extra connectors. Leave undefined any used for non-endstop and non-probe purposes.
#define USE_XMIN_PLUG
#define USE_YMIN_PLUG
#define USE_ZMIN_PLUG
...
#define USE_ZMAX_PLUG // ENABLE IF USING Z_MAX FOR PROBE
````

```cpp

// Mechanical endstop with COM to ground and NC to Signal uses "false" here (most common setup).
...
#define Z_MIN_PROBE_ENDSTOP_INVERTING false // Set to true to invert the logic of the probe.
```


```cpp
//===========================================================================
//============================= Z Probe Options =============================
//===========================================================================
// @section probes

//
// See https://marlinfw.org/docs/configuration/probes.html
//

/**
 * Enable this option for a probe connected to the Z-MIN pin.
 * The probe replaces the Z-MIN endstop and is used for Z homing.
 * (Automatically enables USE_PROBE_FOR_Z_HOMING.)
 */
// #define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN // 

...

/**
 * Z_MIN_PROBE_PIN
 *
 * Define this pin if the probe is not connected to Z_MIN_PIN.
 * If not defined the default pin for the selected MOTHERBOARD
 * will be used. Most of the time the default is what you want.
 *
 *  - The simplest option is to use a free endstop connector.
 *
 *  - RAMPS 1.3/1.4 boards may use the 5V, GND, and Aux4->D32 pin:
 *    - For simple switches connect...
 *      - normally-closed switches to GND and D32.
 *      - normally-open switches to 5V and D32.
 */
#define Z_MIN_PROBE_PIN PA4 // Pin 32 is the RAMPS default
                            // Our Ender-3 test printer with Creality 4.2.2 controller
                            // uses the filament runout sensor connector 
````


Marlin has a few probe deploy strategies built in. The one that we have found to work the best is the Allen Key Probe module. 

Once the deploy and retract strategies are defined in the firmware, then the execution is automatic on demand. 

The full board setup, probe and Allen Key setup are bundled in the Ender3 config files as example. 

{% include note.html content="Marlin stepwise deploy and stow strategy is not difficult. The challenge is the tedious nature of writing it into the firmware config file and recompiling.  Users are encouraged to work out the gcode movements as much as they can as a standalone scripts before entering it into the firmware and recompiling." %}

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

