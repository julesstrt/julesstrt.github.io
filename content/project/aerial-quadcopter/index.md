---
title: "Aerial Robotics: Quadcopter Project"
summary: "Hardware project (EPFL MICRO-502) — trajectory planning and control of a quadcopter in a custom-built obstacle course."
date: 2024-01-01
tags: ["Robotics", "Aerial Robotics", "Trajectory Planning"]
image:
  caption: ""
  focal_point: "Smart"
---

Hardware project for the EPFL MICRO-502 course, completed in a team of five (Mark El Hage, Laetitia Fayad, Aurélien Genin, Maxime Risse, Jules Streit).

A quadcopter had to autonomously navigate through a series of gates set up in a physical obstacle course.

**Key elements:**
- Waypoint generation before and after each gate, with a fixed clearance
- Linear interpolation between setpoints for simple waypoints
- Catmull-Rom spline interpolation for smooth path planning, with configurable segment density between waypoints
- Comparison between simple waypoint-based trajectories and smoothed spline trajectories
