---
title  : "MPAS OpenACC"
date   : 2022-05-03T09:23:17-06:00
type   : software
tagline: "MPAS OpenACC"
docs   : "https://geocat.ucar.edu/"
repo   : "https://github.com/MPAS-Dev/MPAS-Model"
image  : "images/backgrounds/Earth_grid.jpeg"
---


Model for Prediction Across Scale (MPAS) 
Model for Prediction Across Scale is global meteorology and climate simulation model which consists of various components like atmosphere, ocean, sea-ice, land model along with appropriate physics packages to model various quantities of earth system.  The Model for Prediction Across Scales - Atmosphere (MPAS-A) code is the primary atmospheric simulation code inside MPAS.  
In this paper, we present the details about MPAS-A code, details about various resolutions, challenges and strategies to accelerate the dynamical core of MPAS-A using a directive-based programming model (OpenACC) in order to achieve performance portability and maintain a single source code for both CPUs and GPUs execution. 

And finally the results of the porting efforts are discussed in the results section which includes the performance comparison of MPAS-A simulation at 120km, 60km, 30km, 15km, 10km, 5km, 3km. On an average, MPAS-A dynamical core performance with the optimized routines achieves 3.7x speedup using a NVIDIA V100 GPU over a fully subscribed 36-core Intel Broadwell CPU node. In other words, the performance of the dynamical core on a single NVIDIA V100 GPU is equivalent to 130 Broadwell cores. We also measure parallel performance on up to 4200 GPUs and present weak and strong scaling results
