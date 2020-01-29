---
layout: project-individual
title: Object detection benchmarking
---

# Exploring varied object detection architectures

<div class="card">
    <div class="iframe-container">
        <iframe src="https://www.youtube.com/embed/-MSS-DaxShg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>        
    </div>    
    * Videos have been sped up so that it is not so boring! I set the faster clip to 30 FPS and the other
    at 9.4 FPS, so the proportional speed still maintains.
</div>

When deploying machine learning models to the real world, specially in resource constrained environments, 
then model size and complexity plays a big role into determining it's usability, i.e.: will it make
predictions that are correct and also in a reasonable time? 

In order to have a general idea of the impact that your hardware has on **processing time** for the object detection task, I'm presenting to you
a preliminary benchmark table on a set of 1600 JPEG frames with 1280x720 resolution on the following hardware:

| Hardware | CPU | RAM | Graphics card |
|----------|-----|-----|------------|
| Raspberry Pi 3 B+ | 1.4GHz 64-bit quad-core ARM Cortex-A53 CPU | 1GB LPDDR2 SDRAM | None | 
| Raspberry Pi 3 B+ | 1.4GHz 64-bit quad-core ARM Cortex-A53 CPU | 1GB LPDDR2 SDRAM | Movidius Neural Compute Stick (not a video card, but helps for GPU processing) |
| Dell G3 15 | Intel(R) Core(TM) i5-8300H CPU @ 2.30GHz | 8GB SODIMM DDR4 Synchronous | GeForce GTX 1050 Mobile |

And the results for a MobileNet with SSD architecture with 22.1 MB:

| Hardware | FPS | Time per frame (s)|
|----------|-----|-------------------|
| Raspberry Pi 3 B+ on CPU | 1.479 | 0.676 |
| Raspberry Pi 3 B+ with Movidius NCU | 4.721 | 0.212 |
| Dell G3 15 on GPU | (TODO) | (TODO) |

