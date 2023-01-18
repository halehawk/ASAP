---
title  : "MURaM IO"
date   : 2023-01-10T10:32:41-07:00
type   : software
tagline: "Adding asynchronous IO to MURaM"
docs   : ""
repo   : ""
image  : "images/backgrounds/philipp-katzenberger-iIJrUoeRoCQ-unsplash.jpg"
---
MURaM from NCAR HAO group is a numerical model to simulate star's magnetic fields and their violent eruptions. 

The MURaM IO is a project to improve scientific data Input/Output (IO) flexibility and performance of MURaM. MURaM originally has native MPIIO to output binary files on each time step.

With advanced IO technology around and scientific post-processing requests, our engineers and students work together developing an asynchronous IO strategy to MURaM by utilizing ADIOS2 IO library developed by ORNL, and outputting to Python Zarr files for easy  analysis on our jupyterhub. At the same time, those MURaM Zarr files are compressed by our in-house lossy compressor SPERR to save up to 5x data storage.  
