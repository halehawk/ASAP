---
title  : "CLUBB"
date   : 2022-05-03T09:23:17-06:00
type   : software
tagline: "CLUBB OpenACC"
docs   : "https://carson.math.uwm.edu/larson-group/clubb_site/about.html"
repo   : "https://github.com/larson-group/clubb_release"
image  : "images/backgrounds/cloud.jpg"
---

CLUBB (Cloud Layers Unified By Binormals) is a parameterization of subgrid-scale (i.e. unresolved)
variability in atmospheric models (Golaz et al. 2002a; Larson and Golaz 2005; Bogenschutz et al.
2013; Larson et al. 2019). CLUBB parameterizes clouds and turbulence, but it is more general than
that. It also parameterizes the subgrid variability in hydrometeors, and in principle it could be
extended to parameterize variability in aerosol-related processes or radiative transfer.

This work involve porting and optimizing CLUBB code on to GPUs using OpenACC and OpenMP target.

 

