---
title: "Compression"
date: 2023-01-17T11:23:34-07:00
layout: staticpage
---

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

Related publications:

Related software:

