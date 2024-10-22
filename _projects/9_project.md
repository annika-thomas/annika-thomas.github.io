---
layout: page
title: DORI
description: a smart fish doorbell
img: assets/img/dori.png
importance: 4
category: fun
---

Spawning fish struggle to navigate past human-made barriers like dams, disrupting ecosystems. The ‘fish door-
bell’ system in Utrecht, Netherlands, uses a live camera feed to allow tourists and viewers to open the dam when they see fish. However, this framework requires constant human monitoring. Our approach, DORI (Detection of River In-habitants), seeks to replace this with an automated system that detects and classifies fish, signaling the dam to open autonomously. We optimize the runtime and performance of the algorithm by integrating and testing the fish detection performance of the state-of-the-art pre-trained models such as Segment Anything Model (SAM), Fast Segment Anything (FastSAM), Recognize Anything Model (RAM), Tag2Text and Contrastive Language-Image Pre-training (CLIP) for image segmentation and classification in the DORI frame-work.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/dori_pipeline.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Pipeline overview for DORI. At each timestamp t, an image and corresponding timestamp are passed into the algorithm. Luminance of the image is calculated, and if the difference between the current luminance and the average luminance is above a threshold Lthresh, the image is segmented using FastSAM. The segment masks produced by Fast SAM are then classified by CLIP, and if the probability of the class ‘fish’ for any segment mask is greater than 0.5, the doorbell is indicated to be pushed.
</div>

Check out our [Github](https://github.com/annika-thomas/DORI) for example Notebooks and code.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/fish1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/fish2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/fish3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Stills from the fish doorbell, taken from [the fish doorbell webpage](https://visdeurbel.nl/en/the-fish-doorbell/).
</div>

