---
layout: page
title: Soft robotic fish
description: repetitive learning control with soft sensory feedback
# img: assets/img/proj_fish.jpg
importance: 4
category: research
related_publications: true
---

At the **Max Planck Institute for Intelligent Systems** in Stuttgart, in the Locomotion in
Biorobotic and Somatic Systems Group, I worked on controlling body-caudal undulation in a soft
robotic fish.

Soft bodies make the usual control assumptions awkward: the plant is compliant, high-dimensional,
and hard to model accurately, but the motion you want is periodic. Repetitive learning control
exploits exactly that periodicity — the controller improves cycle over cycle using embedded soft
sensors as feedback, rather than relying on a model that would be difficult to identify.

This was my master's thesis work, published in Frontiers in Sensors {% cite schwab2024learning %}.
