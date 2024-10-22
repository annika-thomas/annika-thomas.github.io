---
layout: page
title: Spherical Control Moment Gyroscope
description: satellite attitude control system
img: assets/img/scmg_crop.png
importance: 2
category: work
---

The spherical control moment gyroscope is a continuation of work completed by Tyler Hamer, PhD. Hamer’s work involved the construction and validation of a magnetically suspended spherical permanent magnet dipole actuator that operates as a reaction wheel, meaning it actuates in two instantaneous rotational degrees of freedom. My work involved electromagnetics modeling, force and torque modeling, and magnetic suspension that inform how to incorporate inductive spin into the symmetric axis of the spherical rotor so it operates in three instantaneous rotational degrees of freedom.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/scmg_decomposed.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

To model the inductive spin drive, I derived two different models, including a bulk conductivity model and a thin shell current model of the dipole permanent magnet rotor and the surrounding coils. Below shows the simulated fields in Ansys for a dipole configuration (left) and the analytically derived field for a quadrupole configuration (right). 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/em_modeling.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

I designed a closed-loop feedback control system to levitate a permanent magnet rotor prototype. Plant modeling and controller design is shown for closed-loop suspension below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/suspension.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

With the thin shell model (left), I analytically model inductive drive to generate torque depending on the surface material and validate my findings using finite element modeling simulation. For the shell bulk conductivity model (right), I analytically model a copper shell to generate torque and validate my findings using finite element modeling simulation.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/torque-speed.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>
