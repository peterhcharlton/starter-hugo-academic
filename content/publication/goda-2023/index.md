---
title: "pyPPG: A Python toolbox for comprehensive photoplethysmography signal analysis"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Marton A. Goda
- admin
- Joachim Behar

date: "2024-04-08T00:00:00Z"
doi: "10.1088/1361-6579/ad33a2"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: Physiological Measurement
publication_short: Phys Meas.

abstract: Objective&#58; Photoplethysmography is a non-invasive optical technique that measures changes in blood volume within tissues. It is commonly and being increasingly used for a variety of research and clinical applications to assess vascular dynamics and physiological parameters. Yet, contrary to heart rate variability measures, a field which has seen the development of stable standards and advanced toolboxes and software, no such standards and limited open tools exist for continuous photoplethysmogram (PPG) analysis. Consequently, the primary objective of this research was to identify, standardize, implement and validate key digital PPG biomarkers. Approach&#58; This work describes the creation of a standard Python toolbox, denoted pyPPG, for long-term continuous PPG time-series analysis and demonstrates the detection and computation of a high number of fiducial points and digital biomarkers using a standard fingerbased transmission pulse oximeter. Main results&#58; The improved PPG peak detector had an F1-score of 88.19&#37; for the state-of-the-art benchmark when evaluated on 2054 adult polysomnography recordings totaling over 91 million reference beats. The algorithm outperformed the open-source original Matlab implementation by approximately 5&#37; when benchmarked on a subset of 100 randomly selected MESA recordings. More than 3000 fiducial points were manually annotated by two annotators in order to validate the fiducial points detector. The detector consistently demonstrated high performance, with a mean absolute error of less than 10 ms for all fiducial points. Significance&#58; Based on these fiducial points, pyPPG engineered a set of 74 PPG biomarkers. Studying PPG time-series variability using pyPPG can enhance our understanding of the manifestations and etiology of diseases. This toolbox can also be used for biomarker engineering in training data-driven models. pyPPG is available on https://physiozoo.com/.

# Summary. An optional shortened abstract.
summary: A Python toolbox for comprehensive photoplethysmography signal analysis

tags:
- photoplethysmography
- signal processing

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
- name: Submitted manuscript
  url: https://doi.org/10.48550/arXiv.2309.13767

url_pdf: 'https://iopscience.iop.org/article/10.1088/1361-6579/ad33a2/pdf'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: **M.A. Goda et al.** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- understanding ppg
- vascular ageing
---

## The toolbox

The pyPPG toolbox is available [here](https://pyppg.readthedocs.io/en/latest/).

---
