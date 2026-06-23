---
title: "Deep Learning: Image Processing for Earth Observation"
summary: "Hurricane damage classification from satellite imagery, comparing three CNN architectures and evaluating model calibration alongside raw accuracy."
date: 2025-09-01
tags: ["Deep Learning", "Remote Sensing", "Computer Vision", "Model Calibration"]
image:
  caption: ""
  focal_point: "Smart"
---

Deep learning project for post-disaster damage assessment from satellite imagery.

**Data:** RGB satellite patches of areas in Texas after Hurricane Harvey, captured by the GeoEye-1 satellite. Two classes: damage / no damage. 19,000 training images (unbalanced), 2,000 validation and 2,000 test images (both balanced) â€” with the validation/test sets including visually ambiguous or lower-quality samples to reflect realistic, noisy post-disaster conditions.

**Models trained:**
- QUOC (trained from scratch)
- ResNet (ImageNet pre-trained, fine-tuned)
- VGG (ImageNet pre-trained, fine-tuned)

**Recalibration techniques applied to each model:**
- Platt scaling
- Temperature scaling
- Isotonic regression

**Evaluation:**
- Classification performance: confusion matrix, F1-score, accuracy
- Calibration: reliability curves, Brier score, Expected Calibration Error (ECE)

In the context of hurricane damage detection, particular attention was paid to minimizing false negatives.

