---
type: Article
title: "2020 12 08 Enhanced Headroom Plot In R 9273Ffdf163A"
description: ""
resource: "authors/virtual_adrianco/medium_adrianco/2020-12-08_Enhanced-headroom-plot-in-R-9273ffdf163a.txt"
tags:
  - article
---

# 2020 12 08 Enhanced Headroom Plot In R 9273Ffdf163A






## Excerpt

[URL] https://medium.com/@adrianco/2020-12-08_Enhanced-headroom-plot-in-R-9273ffdf163a

Enhanced headroom plot in R

Imported from a Blogger post I wrote in 2008. Code shared on GitHub

For some reason I seem to find time to write code in R when I’m on an airplane. The last two trips I made resulted in significant enhancements and debugging of the code for my headroom plot. It started off simple but it now has a lot of bells and whistles, including color coding.

Main changes: the quantile used to remove outliers now only removes outliers that exceed the 95th percentile response time by default. It keeps all the throughput values unless you use qx=True.

In each of the throughput bins used to draw the histogram, the maximum response time for that bin is now calculated and displayed as a staircase line unless you set max=False.

The set of data is now split into ranges and color coded. The times series plot is coded so you can see the split, and the scatterplot shows how those points fall. I have been plotting weekly data at one minute intervals with split=7, which looks pretty good.

I read in some data that has been extracted from vxstat into a csv format and plotted it three ways
...


## Sources

[1] Source file: authors/virtual_adrianco/medium_adrianco/2020-12-08_Enhanced-headroom-plot-in-R-9273ffdf163a.txt
