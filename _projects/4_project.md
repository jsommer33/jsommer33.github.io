---
layout: page
title: MRI-Compatible Steerable Catheter System for Laser Prostate Surgery
description: Handheld and robotic steerable catheter platform for HoLEP using advanced nitinol fabrication and MRI-compatible design
img: /assets/img/projects/holep-hero.jpg  # Replace with actual hero image
importance: 4
category: medical robotics
related_publications: false
---

## Background & Clinical Motivation

Holmium Laser Enucleation of the Prostate (HoLEP) is an effective treatment for benign prostatic hyperplasia (BPH), but its clinical adoption is limited due to the technical complexity of current tools and restricted access to certain prostate regions.

To address this, I collaborated with clinicians to design a more intuitive, steerable catheter system capable of operating in MRI environments and reaching challenging anatomical areas with improved precision.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/holep-concept.jpg" title="Clinical concept sketches" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Concept sketches illustrating catheter placement in the prostate for HoLEP.
</div>

---

## Custom Handheld Tool with Clinical Feedback

The first stage of development focused on building a handheld catheter system designed through iterative clinician feedback. A custom ergonomic handle was created to actuate the steerable catheter manually, incorporating MRI-compatible tracking coils and intuitive tendon routing.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/holep-handle.jpg" title="Handheld catheter assembly" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  CAD rendering and prototype photo of the handheld catheter system.
</div>

---

## Advanced Nitinol Catheter Manufacturing

The catheter features several segments of varying stiffness, joined using thermal bonding. To enable steerability and tendon-driven control, a multi-step nitinol processing pipeline was developed:

- **Heat Setting:** Nitinol tubes were shaped using thermal fixtures to achieve predefined curvature and elastic response.
- **Femtosecond Laser Micromachining:** High-resolution slotting and bevel cutting enabled localized flexibility and directional deflection.
- **Nitinol-to-Tendon Welding:** Robust welds between nitinol tubing and tendon wires ensured reliable force transmission without slippage.

Each step was validated for strength, MRI-compatibility, and smooth navigation within anatomical phantoms.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/holep-nitinol.jpg" title="Laser machining and welded joints" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Microscopy of laser-cut catheter slots and heat-set curvatures; inset shows tendon-nitinol weld.
</div>

---

## Robotic System for Actuation

To support robotic control, a pneumatic actuation platform was developed to replicate the handheld operations—pulling tendons, translating the catheter, and rotating about its axis. Encoders were integrated to allow precise position tracking and repeatable motion. The system was tested in benchtop conditions using anatomical phantoms.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/holep-robot.jpg" title="Robotic platform and catheter integration" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Robotic actuation system for tendon pulling and catheter control with integrated feedback.
</div>

---

## Control Strategy

Two complementary control approaches are planned for future system integration:

1. **Model-Based Control:**  
   Uses modal kinematics and constrained optimization to plan motion within anatomical bounds.

2. **Model-Less Feedback Control:**  
   Leverages tracking coil data to estimate tip behavior and adjust inputs using an empirically derived Jacobian.

Together, these strategies aim to support autonomous or surgeon-in-the-loop targeting in complex prostate geometries.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/holep-control.jpg" title="Control strategy comparison" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Diagram comparing model-based planning to empirical feedback-driven control using MRI-visible tracking coils.
</div>

---

This project lays the groundwork for more accessible and MRI-guided laser prostate surgery using advanced catheter design and robotic actuation tailored for the clinical workflow of HoLEP.
