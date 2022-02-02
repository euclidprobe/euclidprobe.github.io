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
## Probe Accuracy Testing

Little to no application data was available for the types of switches used in Euclid Probe. Therefore, the engineers and designers who created Euclid Probe embarked on their own testing campaign to qualify the switches and the other components used in construction. This includes mechanical accuracy testing of the individual switches, the entire probe assembly, and actual probe deployment and probe docking cycles on our test printers.

To date, over 500,00 probe deploy-probe-retract cycles with a moving Z-axis dock have been performed. The only probe docking failures were due to operator error: not updating the probe Z-offset between sample changes.

The gathered data was compiled and analyzed to compare the performance between different switch manufactures and models. The overall results have been quite revealing- the usual suspects are not as accurate as they are purported to be, and the other brands and models often dismissed are actually quite accurate.  

Repeatabilities often approach 0.0001mm.  

Here is an example of a single switch’s probing results performed at room temperature. Note the trends of the blue vertical bars showing the trigger point in the speed ranges noted at the top.   

Also not the population of the probe points in relationship to the standard of deviation bars noted in orange. The standard of deviation bars are for the total population.  
<img 
  src="images\00-ProbeTest57_19_45-768x559.png?crop=0.672xw:1.00xh;0.166xw,0&resize=640:*" 
  data-modal 
/>
<!--
<img src="images\00-ProbeTest57_19_45-768x559.png">
-->

## How accurate is Euclid Probe? 
Generally speaking, an order of magnitude more accurate than the nearest competing devices or technologies. 

The probing results will vary based on the firmware and mechanical system of the printer, but we have seen repeatabilities  approaching 0.0005mm.  

Below is a bed map submitted by a user who was convinced that Euclid Probe was being influenced by the bed magnets. Note that the Z variation is inverted (what is 'low' is actually being displayed 'hi').


After some consulting with the user, we advised them to place paper shims over the magnets to determine if there was a hollow over the top of the magnet which would draw down the steel build plate. The results were that the steel build surface was truly being drawn into the hollow above the recessed magnets. The user the carefully shimmed each magnet with paper and cigarette rolling paper shims to level the bed.  This was their result- 

<img 
  src="images\00-accuracyA.png??crop=0.150xw:0.150xh;0.0833xw,0&resize=2560:*" 
  data-modal 
/>

/>
<img 
  src="images\00-accuracy-fixed.png?crop=0.672xw:1.00xh;0.166xw,0&resize=640:*" 
  data-modal 
/>

<img 
  src="https://icatcare.org/app/uploads/2018/06/Layer-1704-1200x630.jpg" 
  data-modal 
/>
<img 
  src="https://hips.hearstapps.com/hmg-prod.s3.amazonaws.com/images/golden-retriever-royalty-free-image-506756303-1560962726.jpg?crop=0.672xw:1.00xh;0.166xw,0&resize=640:*" 
  data-modal 
/>

<script>
  document.querySelectorAll("img[data-modal]").forEach((img) => {
    var content = document.createElement("div"); //background
    content.className = "modal-content";
    content.appendChild(new Image()).src = img.src; //modal image
    img.insertAdjacentElement("afterend", content); //insert invisible content after image
    img.addEventListener("click", () => { //show modal on click
      content.style.opacity = "1";
      content.style.zIndex = "100";
      document.documentElement.style.overflow = "hidden"; //prevent scrolling while modal is shown
    });
    content.addEventListener("click", () => { //hide modal
      content.style.opacity = "";
      content.style.zIndex = "";
      document.documentElement.style.overflow = "";
    });
  });
</script>