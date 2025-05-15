---
layout: page
title: Physiologically Accurate Clot Fabrication for Intracerebral Hemorrhage Evacuation Testing
description: Repeatable, MRI-visible, and mechanically accurate clots for surgical testing of ICH evacuation systems
img: /assets/img/projects/clot-fab-hero.jpg  # Replace with actual hero image
importance: 3
category: medical robotics
related_publications: false
---

## Overview

Intracerebral hemorrhage (ICH) is among the deadliest forms of stroke, and the development of minimally invasive evacuation tools—particularly robotic systems—requires accurate, testable models of clot behavior in the brain. Most prior models reproduce visual or symptomatic features of ICH but fail to replicate the mechanical and spatial conditions required for surgical removal.

This project presents a novel clot fabrication method designed specifically for evaluating ICH evacuation systems.

---

## Fabrication Technique

Clots were formed using a **balloon-guided cavity creation** and **pre-clotted blood injection** protocol. A Foley catheter was inserted into the brain parenchyma, and the balloon was inflated to gently displace tissue and create a defined cavity. Then, **mechanically relevant blood clots** (formed externally using thrombin and calcium chloride) were injected into the void to simulate a localized hematoma.

- Volume: ~10 mL  
- Retention: 98% volume after 2 hours  
- Application: Ex vivo and in vivo testing

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/clot-schematic.jpg" title="Clot fabrication schematic" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Schematic of the clot fabrication process, including balloon expansion and clot injection steps.
</div>

---

## Ex Vivo Validation

The technique was validated in **six excised ovine heads**. CT imaging was used to monitor clot volume over time (30, 60, 90, 120 minutes). All clots showed high retention, and successful evacuation was achieved using a **pneumatic aspiration system**.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/clot-ct-series.jpg" title="CT segmentations of clot volume over time" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  CT scan segmentations showing stable clot retention across 2 hours.
</div>

### Mechanical Testing

Post-experiment, clot samples were subjected to unconfined compression testing. Tangent stiffness values at 75% strain were within the reported physiological range of ICH thrombi (30–80 kPa).

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/clot-mechanics.jpg" title="Mechanical testing setup and stress-strain curve" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Compression rig with overlaid stress-strain curve from mechanical testing.
</div>

---

## In Vivo Demonstration

A **preliminary in vivo study** was performed in a live sheep. Using autologous blood and a modified injection workflow, a 4.03 mL clot was successfully fabricated and visualized using **T2-weighted MRI**.

Evacuation failed due to excessive clot stiffness caused by over-thrombinization, but the test demonstrated feasibility of the approach in surgical settings.

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/clot-mri.jpg" title="In vivo MRI slice with segmented clot" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  T2-weighted MRI showing a 4.03 mL clot fabricated in vivo and segmented for validation.
</div>

---

## Summary Results

A summary of clot fabrication consistency across heads:

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/projects/clot-results-table.jpg" title="Summary of clot fabrication results" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Summary table showing fabricated clot volumes, retention rates, and evacuation outcomes in 4 test heads.
</div>

---

This platform enables **repeatable, controlled, and physiologically relevant ICH models**, helping bridge the gap between benchtop development and clinical translation of next-generation evacuation technologies.

