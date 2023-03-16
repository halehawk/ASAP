---
title  : "EarthWorks"
date   : 2023-02-24T10:42:21-07:00
type   : software
tagline: "EarthWorks:  Climate Modeling at Storm-Resolving Resolutions"
repo   : "https://github.com/EarthWorksOrg/EarthWorks"
image  : images/backgrounds/ewMain.jpg
---

EarthWorks’ goal is to develop a version of an Earth System Model (ESM) model that can run with a grid spacing of just a few kilometers. That’s a significant advancement, considering CESM typically is used with 25- to 100-kilometer grid spacing. The finer resolution will be able to render important geographical features, such as individual large mountains, that play an important role in weather and climate. Coastlines, lakes, and vegetation also will be better represented, and many complex chemical and physical processes will be simulated in a more natural way.

For example, to fully explore how tropical cyclones might change with a changing climate, you need a model with high enough resolution to explicitly simulate the cyclones along with the full complexity of an Earth system model. You also need to be able to run the model for a long enough time period to detect how increasing greenhouse gases will affect cyclones in the future.

Atmospheric models for forecasting weather run at a resolution high enough to accurately capture the formation and evolution of individual cyclones, but they typically aren’t used with a complete representation of atmospheric, oceanic, and surface processes, and they are run for short periods of time.   

Recent computing advances – including the use of graphical processing units, or GPUs, for scientific applications – make the project possible, along with experts in the field. GPUs, originally used to render 3D video games, can help speed up Earth system models by solving equations for many different grid points simultaneously.  The ASAP group is involved with modifying the code within the Earth System Model in order for it to run on GPUs.  This is done by rewriting code to increase parallelization, adding code directives, and optimizing memory movement between the CPU's and GPU's memory devices.  This is needed in order for scientists to be able to simulate climate at a rate of 1/2 of a day simulated for each 24 hours running on the supercomputer.    

This work is sponsored through the National Science Foundation and is led through Colorado State University.
{{< figure src="/images/projects/nsf_logo.png" width="100">}}
{{< figure src="/images/projects/ew_contributors.png" width="300">}}

