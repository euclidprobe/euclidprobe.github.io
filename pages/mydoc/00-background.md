---
title: "Euclid Probe Origins, Technology and Accuracy"
keywords: probe dock, tool mount
tags: [FAQ]
permalink: 00-background.html
sidebar: mydoc_sidebar
folder: mydoc
toc: false
summary: Background 
---

## Our inspirations

The initial design and foundations were laid when the creator purchased a Wanhao Duplicator and was plagued with inconsistent first layers and sought to add a Z-probe to the printer with the hopes improving it. The first probe created was an adaptation of the 'semi-automatic probe' (https://www.thingiverse.com/thing:315698). The initial probe was a hard wired, hand deployed endstop switch on a clamp. While this worked well, it was tedious to mount and un-mount. Instead of clamping the probe body to the carriage, magnets were used to attach and register it to the steel carriage where the cooling fan supports were. 

Then, seduced by the siren's song of better probes, a number of other devices were tried that showed promise and were reputed to be more user friendly. Ultimately, nothing seemed to work as well matching the accuracy that the microswitch provided.

The Euclid Probe was was then adapted for use with RepRap Firmware and wesc's CroXY 3D Printer (https://github.com/CroXY3D/CroXY), and then adapted to Eustathios-Spider V2 (https://github.com/eclsnowman/Eustathios-Spider-V2.5). 

Euclid Probe has since been successfully been implemented on Railcore, Ender3, Ender5, V-Core3/Rat-rig, Voron 2.4 and Wanhao Duplicator i3 printers. Various mount files are included in the CAD and stl folders.

## Probe Accuracy Testing

Little to no application data was available for the types of switches used in Euclid Probe. Therefore, the engineers and designers who created Euclid Probe embarked on their own testing campaign to qualify the switches and the other components used in construction. This includes mechanical accuracy testing of the individual switches, the entire probe assembly, and actual probe deployment and probe docking cycles on our test printers.

To date, over 500,00 probe deploy-probe-retract cycles have been performed. The only probe docking failures were due to operator error- not updating the probe Z-offset dimensions between sample changes.
The gathered data is compiled and analyzed to compare the performance between different switch manufactures and models. The overall results have been quite revealing- the usual suspects are not as accurate as they are purported to be, and the brands and models often dismissed are actually quite accurate.

Here is an example of a single switch’s probing results performed at room temperature.

<img src="images\00-ProbeTest57_19_45-768x559.png">