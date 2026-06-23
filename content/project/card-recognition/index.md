---
title: "Image Analysis and Pattern Recognition"
summary: "Classical computer vision pipeline to detect and classify playing cards from a single RGB image of a table, despite complex backgrounds and occlusions."
date: 2026-04-01
tags: ["Computer Vision", "Image Processing", "Pattern Recognition"]
image:
  caption: ""
  focal_point: "Smart"
---

Classical (non deep-learning) computer vision project to read the state of a card game from a single overhead photo.

**Input:** a single RGB image of a playing table
**Output:** each player's cards (color and value/action), and the active player

**Main challenges:**
- Complex, textured backgrounds
- Dark cards
- Overlapping cards
- Varying lighting conditions
- Partial occlusions

**Pipeline:**
1. Background classification
2. Active player detection (HSV thresholding â†’ morphological opening â†’ blob selection â†’ centroid-to-player mapping)
3. Background removal (HSV thresholding, opening/closing, contour fill)
4. Image segmentation into per-player regions
5. Card detection (color masks, quad/rectangle extraction, fragment pairing, edge-based reconstruction)
6. Card classification (color and value)

