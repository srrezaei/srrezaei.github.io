---
layout: page
title: FPGA nonlinear control
description: nonlinear control of active rectifiers on programmable hardware
# img: assets/img/proj_fpga.jpg
importance: 5
category: engineering
---

At the Center for Power Electronics and Drives (C-PED) in Rome, I developed and tested
**FPGA-based nonlinear control for active rectifiers**.

Power electronics imposes a hard constraint that most control work avoids: the control law has to
execute at switching frequency, in fixed-point arithmetic, on hardware with no operating system.
Implementing a nonlinear controller under those conditions is a useful discipline — it forces you
to account for exactly how much computation a guarantee actually costs.
