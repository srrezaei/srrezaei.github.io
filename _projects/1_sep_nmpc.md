---
layout: page
title: SEP-NMPC
description: safety-enhanced passivity-based NMPC for UAV slung-payload transport
# img: assets/img/proj_sep_nmpc.jpg   # <- add a figure or GIF here
importance: 1
category: research
related_publications: true
---

A quadrotor carrying a cable-suspended payload is underactuated and awkward: the load swings, the
cable alternates between taut and slack, and the coupled dynamics resist the usual separation into
independent position and attitude loops. Two things you want from a controller for this system —
provable stability and provable safety — normally pull against each other.

SEP-NMPC combines **passivity-based control**, which supplies the stability argument, with
**control barrier function** constraints inside a nonlinear MPC formulation, which supply the
safety argument. The result keeps both guarantees simultaneously rather than trading one for the
other, and runs fast enough to close the loop in real time.

The work was accepted to ICRA 2026 {% cite rezaei2026sepnmpc %}.

<!-- Suggested additions once you have them:
     - a GIF of the payload tracking a trajectory
     - a plot of the barrier function staying non-negative through an aggressive maneuver
     - a link to the arXiv preprint and the code
-->
