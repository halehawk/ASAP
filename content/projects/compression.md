---
title: "Compression"
date: 2023-01-18T09:19:37-07:00
type: projects
image: "images/backgrounds/soccer.jpg"
category: ["RESEARCH"]

---


**Summary**

Climate models such as the Community Earth System Model (CESM)
 typically produce enormous amounts of output data, and storage
 capacities have not increased as rapidly as processor speeds over the
 years. As a result, the cost of storing huge data volumes has become
 increasingly problematic and has forced climate scientists to make
 hard choices about which variables to save, data output frequency,
 simulation lengths, or ensemble sizes, all of which can negatively
 impact science objectives. Therefore, we have been investigating
 lossy data compression techniques as a means of reducing data storage
 for CESM.  Lossy compression, by definition, does not exactly
 preserve the original data, but it achieves higher compression rates
 and subsequently smaller storage requirements. However, as with any
 data reduction approach, we must exercise extreme care when applying
 lossy compression to climate output data to avoid introducing
 artifacts in the data that could affect scientific conclusions.

Our focus has been on better understanding the effects of lossy
 compression on spatio-temporal climate data and on gaining user
 acceptance via careful analysis and testing. To that end, we are
 developing appropriate climate-specific metrics and tools to enable
 scientists to evaluate the effects of lossy compression on their own
 data and facilitate optimizing compression for each variable. For
 example, the  Large Data Comparison for Python (LDCPy) package for visualizing
and computing statistics on differences between multiple datasets,
which enables climate scientists to discover potentially relevant
compression-induced artifacts in their data.

{{< figure src="/images/projects/data.png" caption="This figure illustrates data growth at NCAR from July 2018 to February 2022." width="700">}}

**Related software:**

https://github.com/NCAR/ldcpy

**Related publications:**

H. Sather, A. Pinard, A.H. Baker, and D.M. Hammerling, “What can real information content tell us about compressing climate model data?” 8th International Workshop on Data Analysis and Reduction for Big Scientific Data (DRBSD-8), 2022, to appear.

Alexander Pinard, Dorit M. Hammerling, Allison H. Baker. “Assessing Differences in Large Spatio-temporal Climate Datasets with a New Python package”, International Workshop on Big Data Reduction (BigData2020), pp. 2699-2707, 2020.

Andrew Poppick, Joseph Nardi, Noah Feldman, Allison H. Baker,
Alexander Pinard, and Dorit M. Hammerling. “A Statistical Analysis of
Lossily Compressed Climate Model Data”, Computers and Geosciences,
vol. 145, 2020.

Dorit M. Hammerling, Allison H. Baker, Alexander Pinard, Peter Lindstrom, "A collaborative effort to improve lossy compression for climate data,” in The Fifth International Workshop on Data Analysis and Reduction for Big Scientific Data, Denver, CO, 2019. 

A.H. Baker, D.M. Hammerling, and T.L. Turton. “Evaluating image quality measures to assess the impact of lossy data compression applied to climate simulation data”, Computer Graphics Forum 38(3), June 2019.

A. H. Baker, H. Xu, D. M. Hammerling, S. Li, and J. Clyne, “Toward a
Multi-method Approach: Lossy Data Co
mpression for Climate Simulation Data”, in J.M. Kunkel et al. (Eds.): ISC High Performance Workshops 2017, LNCS 10524, pp. 30–42, 2017.

Allison H. Baker, Dorit M. Hammerling, Sheri A. Mickelson, Haiying Xu,
Martin B. Stolpe, Phillipe Naveau, Ben Sanderson, Imme Ebert-Uphoff,
Savini Samarasinghe, Francesco De Simone, Francesco Carbone, Christian
N. Gencarelli, John M. Dennis, Jennifer E. Kay, and Peter Lindstrom,
“Evaluating Lossy Data Compression on Climate Simulation Data within a
Large Ensemble.”  Geoscientific Model Development, 9, 4381-4403,  2016.

A.H. Baker, H. Xu, J.M. Dennis, M.N. Levy, D. Nychka, S.A. Mickelson
, J. Edwards, M. Vertenstein, A. Wegener, “A Methodology for Evaluating the Impact of Data Compression on Climate Simulation Data.” Proc. of the 23rd International ACM Symposium on High Performance Parallel and Distributed Computing (HPDC14), Vancouver, CA, pp. 203-214, 2014.



