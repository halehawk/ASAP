---
title: "Correctness and Verification"
date: 2023-01-18T17:00:46-07:00
type: projects
image: "images/backgrounds/markus-spiske-iar-afB0QQw-unsplash.jpg"
category: ["RESEARCH"]
---

**Summary**

Model simulations are essential tools for understanding weather and climate. Many of these models are
the result of multiple years or even decades of development, which has resulted in large and complex
code bases that are still continually evolving. Indeed, most of these codes are in a state of near constant
development, as new scientific capabilities and processes are frequently added and ever-evolving
high-performance computing (HPC) technologies require code adaptations and further optimizations.
Repeated software verification is necessary during the development life cycle to ensure that the changes
made to the hardware and/or software environment do not inadvertently change the model results. For
institutions like the National Center for Atmospheric Research (NCAR), maintaining model confidence
and preserving code quality and reliability is critical given the societal importance of these codes as
we adapt to our changing climate. In fact, climate and weather model simulation output inform both our
understanding and policy decisions in areas such as agriculture, public health, and extreme weather
events.

Maintaining confidence and preserving code quality and reliability of
these climate and weather codes is critical. Given the scale of these models, a thorough correctness evaluation may be prohibitively expensive. It is also customary to require regression tests to yield bitwise identical results. This requirement is often unmet due to the chaotic nature of climate and weather models and the large variety of hardware/software environments they are run on. When bitwise identical results cannot be sought, field experts are to evaluate model results in a time-consuming and subjective manner.
In short, climate and weather modeling communities are in need of
practical and feasible means of ensuring correctness and
reproducibility. For example, we are interested in means to easily assess whether
changes to a model code result in output that is systematically
different or introduce artifacts that could influence scientific
conclusions. Such changes may include hardware or software stack
infrastructure differences, replacing parts of the model with
ML-routines, or applying data compression to the output data.

Determining correctness raises interesting statistical and numerical analysis research questions, and we
have made progress on this front in several areas. For example, the Community Earth System Model
Ensemble Consistency Test (CESM-ECT) suite was developed as an alternative to requiring bitwise
identical output for quality assurance (Baker, 2015; Baker, 2016; Milroy, 2018). This objective test does
not determine correctness per se, but instead answers the more tangible question: Is the new output
statistically distinguishable from the original? Ensemble methods are common in climate studies, as a
collection of simulations are needed to describe the natural variability in the climate model system. In
particular, CESM-ECT provides a statistical measurement of consistency between a large “baseline”
ensemble (on a trusted machine and software stack) and a set of new simulations (for example, from a
new machine, compiler upgrade, optimization, etc.). CESM-ECT utilizes a testing framework based on the
popular technique of Principal Component Analysis (PCA) to determine whether the new simulations are
statistically distinguishable from the baseline ensemble. This ensemble-based approach to verification
serves as a powerful classification tool when bit-identical requirements are too restrictive, and the
CESM-ECT tools are regularly used by CESM software engineers for evaluating ports to new machines,
software upgrades, and modifications that should not affect the climate.

**Related software:**

https://github.com/NCAR/PyCECT

**Related publications and tech notes:**

Dong Ahn, Allison H. Baker, Michael Bentley, Ian Briggs, Ganesh
 Gopalakrishnan, Dorit M. Hammerling, Ignacio Laguna, Gregory L. Lee,
 Daniel J. Milroy, Mariana Vertenstein, "Keeping Science on Keel When
 Software Moves", Communications of the ACM, Volume 64, Number 2,
 pp. 66-74, January 2021.
 

Daniel J. Milroy, Allison H. Baker, John M. Dennis, Andrew Gettelman, and Dorit M. Hammerling, "Investigating the Impact of Mixed Precision on Correctness for a Large Climate Code", in IEEE/ACM 3rd International Workshop on Software Correctness for HPC Applications (Correctness), Denver, CO, USA, pp. 44-51, 2019. 

Daniel J. Milroy, Allison H. Baker, Dorit M. Hammerling, Youngsung
Kim, Thomas Hauser, and Elizabeth R. Jessup, “Making root cause
analysis feasible for large code bases: a solution approach for a
climate model”, Proceedings of the 28th International Symposium on
High-Performance Parallel and Distributed Computing:  HPDC2019,
Phoenix, AZ.  Jon B. Weissman and Ali Raza Butt and Evgenia Smirni
(Eds.), June 2019, pp. 73-84.


Daniel J. Milroy, Allison H. Baker, Dorit M. Hammerling, and Elizabeth R. Jessup, “Nine time steps: ultra-fast statistical consistency testing of the Community Earth System Model (pyCECT v3.0)”, Geoscientific Model Development, 11, pp. 697-711, 2018.

Allison H. Baker, Daniel J. Milroy, Dorit M. Hammerling, and Haiying
Xu. “Quality assurance and error identification for the Community
Earth System Model”, Proceedings of Correctness’17: First
International Workshop on Software Correctness for HPC Applications
(Correctness’17),.ACM, New York, NY, USA, 6 pages, 2017.

Daniel J. Milroy, Allison H. Baker, Dorit M. Hammerling, John M. Dennis, Sheri A. Mickelson, and Elizabeth R. Jessup, “Towards characterizing the variability of statistically consistent Community Earth System Model simulations.”  Procedia Computer Science (ICCS 2016), Vol. 80, pp. 1589-1600, 2016.

A.H. Baker, Y. Hu, D.M. Hammerling, Y. Tseng, X. Hu, X. Huang, F.O. Bryan, and G. Yang, “Evaluating Statistical Consistency in the Ocean Model Component of the Community Earth System Model (pyCECT v2.0).” Geoscientific Model Development, 9, pp. 2391-2406, 2016.

A.H. Baker, D.M. Hammerling, M.N. Levy, H. Xu, J.M. Dennis, B.E. Eaton, J. Edwards, C. Hannay, S.A. Mickelson, R.B. Neale, D. Nychka, J. Shollenberger, J. Tribbia, M. Vertenstein, and D. Williamson, “A new ensemble-based consistency test for the community earth system model (pyCECT v1.0).” Geoscientific Model Development, 8, pp. 2829–2840, 2015.
