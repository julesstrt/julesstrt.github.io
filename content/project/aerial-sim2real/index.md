---
title: "Aerial Robotics: RL and Sim2Real Transfer"
summary: "Reinforcement learning for a bio-inspired flapping-wing drone, with a focus on transferring policies from simulation to the real platform."
date: 2025-02-01
tags: ["Robotics", "Reinforcement Learning", "Sim2Real", "Aerial Robotics"]
image:
  caption: ""
  focal_point: "Smart"
---

Reinforcement learning project on a bio-inspired flapping-wing drone, tracking 3D setpoints in a motion-capture flight arena.

**Sim2Real approach**, combining:
- A dynamics **model** of the platform
- **Reinforcement learning (RL)** for the high-level policy
- A **low-level controller** for stabilization

To close the simulation-to-reality gap, several techniques were used:
- Domain randomization
- Reward shaping
- History (past observations) as part of the policy input

