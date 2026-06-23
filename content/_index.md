---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'Summary'
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '🤖 About My Work'
      subtitle: ''
      text: |-
        I'm a second-year Robotics MSc student at EPFL, with a minor in Space Technologies. My work focuses on **perception-driven autonomy** — building systems where robots can sense, understand, and act in the real world.

        My projects span **autonomous navigation** (ROS2, SLAM, LiDAR/RGB sensor fusion), **learning-based control** (Reinforcement Learning, Imitation Learning), and **hardware integration** (from motor control and 3D printing to full-stack Docker-based deployment).

        I'm currently working with the EPFL AI team on the LeKiwi robot, developing a ROS2 pipeline for autonomous navigation and manipulation. Feel free to reach out! 😃
    design:
      columns: '1'
---
