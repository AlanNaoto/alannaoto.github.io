---
layout: project-individual
title: Classification annotation tool
description: Cleaning our dirty dataset
---
<link rel="stylesheet" href="assets/css/slideshow.css">

<div class="card">
    <div class="slideshow-container">
        <div class="mySlides fade">
            <!-- <div class="numbertext">1 / 2</div> -->
            <img src="assets/imgs/classification_tool.png" style="width:100%">
            <!-- <div class="text">Caption Text</div> -->
        </div>
        <div class="mySlides fade">
        <!-- <div class="numbertext">2 / 2</div> -->
            <img src="assets/imgs/classification_tool_2.png" style="width:100%">
        <!-- <div class="text">Caption Two</div> -->
        </div>
        <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
        <a class="next" onclick="plusSlides(1)">&#10095;</a>
    </div>
    <br>
    <div style="text-align:center">
        <span class="dot" onclick="currentSlide(1)"></span> 
        <span class="dot" onclick="currentSlide(2)"></span> 
    </div>
    <a href="https://github.com/AlanNaoto/Dataset_GUI_labelling_tool"> <img src="assets/imgs/GitHub-Mark-64px.png" width="5%">
    <b>Take a peek into the source code :hugs: </b></a>
</div>

Building a dataset from scratch is not easy. After collecting the data, which by itself is a hurdle, 
more often than not you will find yourself sadly glazing at *dirty, inconsistent data*, realizing
that you are still not yet done. You need to clean the data. That's where this tool comes in handy!

This is a **graphical interface** built on PyQt5 where you go through each frame and **decide
if that instance is worth keeping or not**. After every traversed frame your decision gets stored in a 
database file through sqlite3. In it's current state the script works specifically for
[CARLA like dataset](https://github.com/AlanNaoto/carla-dataset-runner), but can be extended to other applications by modifying the MainApplication class :+1:



<script src="assets/js/slideshow.js"></script>