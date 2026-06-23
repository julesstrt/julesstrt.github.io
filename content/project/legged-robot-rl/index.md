---
title: "Reinforcement Learning for Legged Robot"
summary: "Learning locomotion and dynamic jumps for a quadruped robot in simulation, combining Central Pattern Generators with reinforcement learning."
date: 2024-09-01
tags: ["Reinforcement Learning", "Legged Robotics", "Control"]
image:
  caption: ""
  focal_point: "Smart"
---

Python-based reinforcement learning project for quadruped locomotion and dynamic motion.

**Capabilities:**
- Jumps (forward, lateral, and twist), using Virtual Model Control (VMC) for landing stability
- Locomotion via a Central Pattern Generator (CPG) combined with reinforcement learning
- Multiple gaits: walk and trot
- Tested on flat ground and slopes

### CPG-RL: Learning a Central Pattern Generator for Quadruped Locomotion

Follow-up work exploring **CPG-RL**, where a reinforcement learning policy learns to modulate the parameters of a Central Pattern Generator (oscillator coupling, amplitude, frequency) rather than directly outputting joint commands — combined with inverse kinematics and PD control to track the resulting foot trajectories, using IMU orientation/velocity and foot contact state as observations.
