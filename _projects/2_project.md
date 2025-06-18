---
layout: page
title: Automated MRI-Based Clot Detection for Robotic ICH Surgery
description: Deep learning pipeline for real-time ICH segmentation and robotic targeting
img: /assets/img/AutoSegment.png  # Replace with real image
importance: 2
category: medical robotics
related_publications: false
---

## Overview

Intracerebral hemorrhage (ICH), a severe and often fatal form of stroke, requires precise intervention to safely remove blood clots from the brain. This project focused on enhancing the robotic treatment of ICH by automating the detection and localization of hemorrhages in MRI images.

Using the publicly available **ATLAS v2.0** dataset, 3D MRI scans were preprocessed and converted into 2D slices, which were used to train a **2D U-Net convolutional neural network** to segment hemorrhagic lesions.

---

## U-Net Model and Training

The U-Net model was trained on axial MRI slices to produce binary segmentation masks for hemorrhagic regions. The network leveraged skip connections and multi-scale feature learning to enable accurate boundary detection with minimal training data.

- **Dice Similarity Coefficient:** 0.969  
- **Centroid localization error:** 0.348 mm (mean)

<div class="row justify-content-center">
  <div class="col-md-6 mt-3">
    {% include figure.liquid path="/assets/img/UNet Model.png" title="U-Net model architecture" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Diagram of the U-Net model used for MRI segmentation, highlighting the contracting and expansive paths with skip connections for precise localization.
</div>

---

## Segmentation and Targeting Accuracy

Segmented lesion masks were post-processed to extract contours and compute the centroid of each clot, forming a critical input for robotic path planning (e.g., concentric tube robot targeting).

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="/assets/img/predvsground2.jpg" title="Ground truth vs. U-Net prediction" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Visual comparison between ground truth lesion masks (top row) and U-Net predictions (bottom row) on test MRI slices.
</div>

<div class="row justify-content-center">
  <div class="col-md-6 mt-3">
    {% include figure.liquid path="/assets/img/DiceScore.jpg" title="Dice & IoU over training epochs" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Model performance over training epochs, achieving a Dice score of 0.969 and IoU of 0.94 on test data.
</div>

---

## Example Output for Robotic Planning

<div class="row justify-content-center">
  <div class="col-md-6 mt-3">
    {% include figure.liquid path="/assets/img/SegmentedLesion.jpg" title="Centroid overlay on MRI" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Example of a lesion overlaid on an MRI slice with predicted contour and centroid (used for robotic targeting).
</div>

---

## Summary

This work lays the groundwork for integrating real-time image segmentation into **autonomous surgical systems**, improving the speed, consistency, and precision of **minimally invasive ICH evacuation** procedures.
