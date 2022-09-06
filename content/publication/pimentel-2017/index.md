---
title: Toward a robust estimation of respiratory rate from pulse oximeters

summary: 'A novel technique for estimating respiratory rate from photoplethysmography signals.'

authors:
- Marco A F Pimentel
- Alistair E W Johnson
- admin
- Drew Birrenkott
- Peter J Watkinson
- Lionel Tarassenko
- David A Clifton
tags: [respiratory rate, wearables, photoplethysmography]
categories: []
date: '2016-11-18'
lastmod: 2022-09-06T16:00:00Z
featured: false
draft: false

url_dataset: 'https://doi.org/10.13026/C2208R'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Source: [**M.A.F Pimentel _et al._**](/publication/pimentel-2017/) ([CC BY 3.0](https://creativecommons.org/licenses/by/3.0/))'
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: [RR wearables]
publishDate: '2022-01-12T22:58:24.891430Z'
publication_types:
- '2'
abstract: 'Goal. Current methods for estimating respiratory rate (RR) from the photoplethysmogram (PPG) typically fail to distinguish between periods of high- and low-quality input data, and fail to perform well on independent "validation" datasets. The lack of robustness of existing methods directly results in a lack of penetration of such systems into clinical practice. The present work proposes an alternative method to improve the robustness of the estimation of RR from the PPG. Methods. The proposed algorithm is based on the use of multiple autoregressive models of different orders for determining the dominant respiratory frequency in the three respiratory-induced variations (frequency, amplitude and intensity) derived from the PPG. The algorithm was tested on two different datasets comprising 95 8-minute PPG recordings (in total) acquired from both children and adults in different clinical settings, and its performance using two window sizes (32 and 64 seconds) was compared with that of existing methods in the literature. Results. The proposed method achieved comparable accuracy to existing methods in the literature, with mean absolute errors (median, 25th-75th percentiles for a window size of 32 seconds) of 1.5 (0.3-3.3) and 4.0 (1.8-5.5) breaths per minute (for each dataset respectively), whilst providing RR estimates for a greater proportion of windows (over 90% of the input data are kept). Conclusion. Increased robustness of RR estimation by the proposed method was demonstrated. Significance. This work demonstrates that the use of large publicly-available datasets is essential for improving the robustness of wearable-monitoring algorithms for use in clinical practice.'
publication: '*IEEE Transactions on Biomedical Engineering*'
doi: 10.1109/TBME.2016.2613124
links:
- name: Full Text
  url: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7748483
  
projects:
- RR wearables
---
