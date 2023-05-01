---
title  : "CM1"
date   : 2022-05-03T09:23:51-06:00
type   : software
tagline: "Adding GPU Support Into CM1"
repo   : "https://github.com/george-bryan/CM1/tree/gpu-opt"
image  : "images/projects/tornadoCM1.png"
---
The Cloud Model version 1 is a mesoscale atmospheric model that
allows for idealized studies of atmospheric phenomena. A new
Lagrangian microphysics capability has been added which enables
a significantly more accurate representation than the traditional
bulk or multi-moment approaches frequently found in mesoscale
atmospheric models. We have utilized a directive-based approach
to enable a single source code to efficiently support the execution of
CM1 on both CPU and GPU-based computing platforms. In addition
to the use of accelerator directives, changes to the index search
scheme and the message-passing algorithms used by the lagrangian
microphysics were necessary to enable efficient execution. We focus
on a configuration of CM1 that will be used to investigate the impact
of oceanic sea spray on the atmospheric boundary layer within
a hurricane. We observe a factor of 2.9x reduction in time to the
solution when between eight NVIDIA A100 GPUs and eight AMD
Eypc based compute nodes

CM1 is a product of the National Center for Atmospheric Research’s MMM Lab. Support for CM1 is provided by the U.S. National Science Foundation 
