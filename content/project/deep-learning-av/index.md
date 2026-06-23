---
title: "Deep Learning for Autonomous Vehicle"
summary: "End-to-end trajectory prediction for autonomous driving, trained on the nuPlan dataset and progressively generalized to real-world sensor data."
date: 2026-03-01
tags: ["Deep Learning", "Autonomous Vehicles", "Computer Vision"]
image:
  caption: ""
  focal_point: "Smart"
---

Deep learning project for trajectory prediction in autonomous driving, structured in three progressive milestones.

**Training sample structure:** a front-facing RGB camera image, history features (past 21 steps), driving command ("forward"/"left"/"right"), and a future trajectory to predict (60 steps), optionally paired with depth and semantic segmentation maps as auxiliary supervision.

**Milestone 1 â€” Basic end-to-end planner**
Trained on a subset of the nuPlan dataset: 5,000 training and 1,000 validation samples (RGB image, history features, driving command, future trajectory).
â†’ Validation ADE: **1.76 m**

**Milestone 2 â€” Perception-aware planning**
Added depth and semantic segmentation maps as auxiliary supervision signals.
â†’ Validation ADE: **1.609 m**, improving over the Milestone 1 baseline

**Milestone 3 â€” Sim-to-real generalization**
Added 900 real-world samples (same trajectory format, captured from real sensors, without depth/semantic annotations) to training and validation sets, with evaluation on real-world images.
â†’ Validation ADE: **1.42 m**, demonstrating strong sim-to-real generalization

