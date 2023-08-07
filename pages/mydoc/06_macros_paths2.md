---
title: "Euclid Macros Paths"
keywords: macros paths
tags: [macros]
last_updated: March 4, 2023
permalink: 06_macros_paths2.html
sidebar: mydoc_sidebar
folder: mydoc
toc: true
summary: Euclid Macros Paths
---
<style>
     #mycanvas{border:1px solid red;}
</style>
https://www.tutorialspoint.com/html5/canvas_drawing_rectangles.htm

<div style="width:100%;text-align:center;">
<canvas id="myCanvas" width="604" height="604" style="border:2px solid #d3d3e3;">
Your browser does not support the HTML canvas tag.</canvas>

 <script type = "text/javascript">
    function drawShape() {

        // Get the canvas element using the DOM
        var canvas = document.getElementById("myCanvas");

        // Make sure we don't execute when canvas isn't supported
        if (canvas.getContext) {

           // use getContext to use the canvas for drawing
           var ctx = canvas.getContext('2d');

           // drawing code here  
           ctx.fillRect(5,5,100,100);
           ctx.clearRect(10,10,60,60);
           ctx.strokeRect(25,25,100,100);
        } else {
           alert('You need Safari or Firefox 1.5+ to see this demo.');
            }
         }
      </script>
</div>

