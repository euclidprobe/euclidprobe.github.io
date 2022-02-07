---
title: "Marlin Firmware settings"
keywords: firmware, settings, offsets
tags: [firmware, offsets]
last_updated: February 5, 2022
permalink: 05_marlin.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Marlin Firmware Settings
---


### Marlin Probe device configuration
Marlin configuration is highly dependent on the controller board used. The following is a general outline of the hardware definition only. The probe deployment and retraction, also part of the Configuration.h file is addressed in the next pages and Ender3 and Ender5 printer examples.

<div style="width:100%;text-align:center;"> 
<a href="images\05_probe-offsets-sm.png" data-lity> <img src="images\05_probe-offsets-sm.png" style="width:450px; border:2px solid CornflowerBlue"></a></div>

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
````

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
