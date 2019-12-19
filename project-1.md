---
layout: project-individual
title: CARLA dataset collector
description: Creating RGB, 2d bounding boxes and depth data
---

<div class="card">
    <div class="iframe-container">
        <iframe src="https://www.youtube.com/embed/LgSwWo82wC0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>    
<br>
<a href="https://github.com/AlanNaoto/carla-dataset-runner"> <img src="assets/imgs/GitHub-Mark-64px.png" width="5%">
<b>Take a peek into the source code :hugs: </b></a>
</div>

[CARLA](http://carla.org/) is an open-source autonomous vehicle driving suite built on top of 
Unreal Engine 4 which provides a Python API to manage the simulations. In this repo, I built a data
collector on top of it, which spawns vehicles, pedestrians, changes the weather to a custom set, and
allocates sensors (RGB, 2D bounding box and depth) on random vehicles to records all data into a 
single HDF5 file.

With the data recorded from this repo, one can **quickly build their own private dataset** to train 
machine learning models for autonomous driving and other applications :blush:
