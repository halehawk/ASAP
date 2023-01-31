---
title: "Sperr_hackathon"
author: ""
date: 2023-01-31T13:42:48-07:00
type: news
image: images/blog/hackathon.png
feature_image: images/blog/hackathon.png
news_images: ["images/projects/project-details-image-one.jpg", "images/projects/project-details-image-two.jpg"]
---

On Feb 21, 2023, members from ASAP group and VAST group will attend OpenACC GPU Hackathons to optimize VAST's SPERR data compressor with GPUs. OpenACC GPU Hackathons are 5-day events designed to help teams of three to six developers accelerate their own codes on GPUs with OpenACC or other tools. SPERR is a C++ library that supports lossy compression of multi-dimensional (one, two, or three) floating-point data. Recent profiling results of SPERR on CPU indicates that of the five most expensive functions, four of them are written in such a way that exposes sufficient parallelism. So in the Hackathons, we are looking for software engineering support to help identify and optimize SPERR to fully utilize GPU performance.
