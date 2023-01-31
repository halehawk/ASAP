---
title: "Just-in-time(JIT) compilation on GPU for atmospheric chemistry"
author: "Jian Sun"
date: 2023-01-30T10:45:59-06:00
type: news
image: images/blog/timur-garifov-26kXlHVtRmc-unsplash.jpg
feature_image: images/blog/timur-garifov-26kXlHVtRmc-unsplash.jpg
layout: staticpage
---

Atmospheric chemistry solvers require efficient calculations of chemical forcing. To avoid using indirect addressing in these calculations, code-generating tools are often used to embed hard-coded indices into mechanism-specific functions. Although these tools result in efficient executables, they greatly complicate the build process and increase maintenance costs for the models, as the code has to be generated and compiled ahead of time (AOT) for every change to a chemical mechanism. In contrast, just-in-time (JIT) compilation can build the necessary chemistry solver at runtime and potentially overcome the drawbacks of AOT compilation. We would like to explore how to (1) optimize a CPU-based JIT-compiled toy forcing function we have developed and (2) enable its execution on both CPU and GPU. Once the new code is available, we will further evaluate the CPU and GPU performance of the JITed code against that of the traditional AOTed code. By doing this, we expect to have a solid understanding of the applicability of JIT compilation to scientific applications and its performance implications, including on GPUs. This will be very helpful as we explore applying JIT compilation to a full chemistry solver. This will be one of the 2023 SIParCS summer intern projects and one project of NOAA/NCAR Open Hackathon.
[More details for 2023 SIParCS](https://www2.cisl.ucar.edu/outreach/internships/2023projects) and [More details for NOAA/NCAR Open Hackathon](https://www.openhackathons.org/s/siteevent/a0C5e000005V8ZlEAK/se000154).

