---
layout: page
title: BeaverCube2 CubeSat
description: Earth-observing nanosatellite
img: assets/img/bc2.png
importance: 1
category: work
related_publications: false
---

BeaverCube2 is a 3U Cube Satellite built in collaboration between MIT STAR Laboratory and Northrop Grumman for experiments involving Earth observation. The satellite is 30 cm x 10 cm x 10 cm in dimension, the CubeSat standard 3U. It hosts one main experiment, the demonstration of a Adaptive Compute Acceleration Platform (ACAP) using two optical sensors and one infrared sensor to study the Earth. 

As the lead mechanical, structural, systems and thermal engineer for BeaverCube2, I designed the satellite to be robust in the launch environment and on orbit. My main contributions are detailed below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/struc2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/struc1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/struc3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Modular computer aided design of all satellite components that successfully integrate all subsystems and meet the size requirements of a 3U CubeSat
</div>

I performed simulations using Ansys to ensure that satellite components can structurally withstand the harsh 13.5G linear accelerations, 8 rad/s radial accelerations, 20,000N side rail loads, and random vibration environment experienced during launch. The design is robust in these conditions. The minimum frequencies of modes of vibration throughout the structure occur well above the allowed minimum mode of 100 Hz. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/vibtest.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Structural analysis of BeaverCube2 in Ansys Mechanical
</div>

I also ensured that all subsystems of the satellite do not reach temperatures exceeding their storage temperature ranges and do not exceed their operating ranges while turned on. Analytical and simulated thermal analysis demonstrates during worst case hot (beta angle) and worst case cold (beta angle) orbits, no subsystem reaches the operating temperature bounds.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/td.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/temps.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Thermal analysis of BeaverCube2 in Thermal Desktop
</div>
