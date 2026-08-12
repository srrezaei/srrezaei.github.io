---
layout: about
title: about
permalink: /
subtitle: >
  Ph.D. Candidate, <a href='https://www.yorku.ca/lassonde/research/space-engineering/'>Department of Earth and Space Science and Engineering</a>,
  <a href='https://www.yorku.ca/lassonde/'>Lassonde School of Engineering</a>, York University.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Spacecraft Dynamics, Control<br>and Navigation Lab (SDCNLab)</p>
    <p>York University</p>
    <p>Toronto, Ontario, Canada</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

I am a Ph.D. candidate in Robotics and Aerospace Engineering at **York University**, working with
Prof. [Jinjun Shan](https://www.yorku.ca/lassonde/research/space-engineering/) in the Spacecraft
Dynamics, Control and Navigation Laboratory (SDCNLab). My research is on making aerial vehicles
carry things safely — specifically, **nonlinear model predictive control** for UAVs transporting
cable-suspended payloads.

A quadrotor with a slung load is a deceptively hard system to control. The payload swings, the
cable goes slack and taut again, the coupled dynamics are underactuated, and the whole thing has to
stay stable while respecting thrust limits and avoiding obstacles. My work combines
**passivity-based control** for stability guarantees with **control barrier functions** for safety,
inside an MPC framework that runs fast enough to close the loop in real time. Recent results include
SEP-NMPC, a safety-enhanced passivity-based controller accepted to ICRA 2026, and ongoing work on
hierarchical NMPC with constraint decomposition.

I care about the distance between a proof and a flying robot. Before York I spent a year at the
**Max Planck Institute for Intelligent Systems** in Stuttgart working on learning control for soft
robotic fish, and I have designed FPGA-based nonlinear controllers for power electronics in Rome.
During my Ph.D. I spent eight months at **Quanser** as a Mitacs-funded research intern, helping
develop and validate the QDrone 2 platform — which means a good deal of my time goes into the
unglamorous work of getting controllers to survive contact with real hardware.

I hold an M.Sc. in Mechatronics Engineering from the University of Rome Tor Vergata and a B.Sc. in
Mechanical Engineering from Shiraz University, with an Erasmus+ exchange at the University of
Stuttgart along the way.
