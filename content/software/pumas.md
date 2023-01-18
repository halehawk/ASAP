---
title  : "PUMAS"
date   : 2023-01-04T15:23:00-06:00
type   : software
tagline: "Adding GPU Support Into PUMAS"
repo   : "https://github.com/ESCOMP/PUMAS"
image  : "images/backgrounds/timur-garifov-26kXlHVtRmc-unsplash.jpg"
---

Parameterization of Unified Microphysics Across Scales, short as PUMAS, is the cloud microphysics parameterization used in the Community Atmosphere Model (CAM).
It is typically a computationally expensive component in an atmospheric model and thus improving its performance could save non-negligible computational resources.
We have utilized the directive-based approach (OpenACC and OpenMP offload) to enable a single source code to efficiently support the execution of PUMAS on both CPU and GPU-based computing platforms in a practical CAM simulation.
Compared to a single compute node (36 CPU cores), using eight GPUs within the same node achieves 3.6x speedup of the PUMAS execution time at 1-degree horizontal resolution (including data movement between CPU and GPU).
This speedup further increases to 5.4x at 0.25-degree resolution, consistent with the fact that GPU favors larger problem size.

Support for CAM and PUMAS are primarily provided by the U.S. National Science Foundation (NSF).
