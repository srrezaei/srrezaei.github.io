---
layout: page
title: Hierarchical NMPC
description: constraint decomposition for safe and stable slung-load transportation
# img: assets/img/proj_hierarchical.jpg
importance: 2
category: research
related_publications: true
---

Enforcing every constraint at every level of a predictive controller is expensive, and often
unnecessary — different requirements are naturally cheapest to satisfy at different levels of the
control hierarchy.

This project decomposes the constraint set across a hierarchy of predictive controllers, assigning
each constraint to the level where it can be enforced most cheaply, without giving up the safety
and stability guarantees that motivated it. The goal is a controller that scales to longer
horizons and richer constraint sets while staying real-time feasible on flight hardware.

In preparation {% cite rezaei2026hierarchical %}.
