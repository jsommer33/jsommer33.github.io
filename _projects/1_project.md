---
layout: page
title: Concentric Tube Robot for ICH Evacuation
description: Minimally invasive MRI-compatible robot for intracerebral hemorrhage removal
img: assets/img/12.jpg
importance: 1
category: medical robotics
related_publications: true
---

## Overview

Intracerebral hemorrhage (ICH) is a form of hemorrhagic stroke caused by the rupture of a blood vessel in the brain, leading to bleeding into brain tissue. With a mortality rate exceeding 50% in the first year and limited surgical options, there is an urgent need for safe and effective minimally invasive interventions. While recent trials like **ENRICH** show promise for surgical evacuation, current tools lack the dexterity and intraoperative feedback required for precise clot removal.

This project focuses on the development and validation of an **MRI-compatible concentric tube robot (CTR)** for minimally invasive ICH evacuation, offering improved dexterity within the brain and the ability to perform under live MRI guidance.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/12.jpg" title="Illustration of ICH location in brain" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

---

## The System

The robot features:

- A pre-curved inner tube nested inside a rigid outer tube, offering 3 degrees of freedom (translation, rotation, curvature).
- A stereotactic aiming platform (**NICE-Aiming**) for precise alignment based on MRI data.
- Custom MRI-compatible actuation using **pneumatic motors** and **fiber optic feedback**.
- A **MATLAB-based control interface** for surgeon-in-the-loop operation.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/12.jpg" title="CTR system diagram and control flow" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

---

## Ex Vivo Experiments

We conducted a comparative study on excised sheep heads to evaluate the performance of the CTR in clot evacuation.

### Clot Fabrication

A 13 mL artificial clot was created by expanding a balloon catheter within the brain to form a cavity, followed by injecting a clot-mimicking material under MRI guidance.

This process ensured the clot’s shape required use of the CTR's curved capabilities—something straight tools couldn’t reach.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/12.jpg" title="Clot cavity formation via balloon expansion" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

### Experimental Procedure

MRI imaging was used to identify clot location and guide robot alignment using **NICE-Aiming**.

Two evacuation approaches were tested:

1. **Straight-only insertion** (mimicking standard endoscopic tools)  
2. **Curved insertion** using the full CTR articulation

Both techniques used **vacuum aspiration** under dynamic MRI feedback.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/12.jpg" title="MRI-guided alignment and evacuation" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

---

## Results

- **Straight-only approach** removed **65.3%** of the clot, leaving difficult-to-reach areas.
- **Curved CTR evacuation** achieved **95.5%** total clot removal, with residual volume under **1 mL**—surpassing the clinically meaningful threshold scaled for sheep anatomy.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/results.jpg" title="Clot removal comparison: straight vs. curved" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
