---
title: "pyPPG: A Python toolbox for comprehensive photoplethysmography signal analysis"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Marton A. Goda
- admin
- Joachim Behar

date: "2023-09-24T00:00:00Z"
doi: "10.48550/arXiv.2309.13767"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: arXiv
publication_short: arXiv

abstract: Photoplethysmography is a non-invasive optical technique that measures changes in blood volume within tissues. It is commonly and increasingly used for in a variety of research and clinical application to assess vascular dynamics and physiological parameters. Yet, contrary to heart rate variability measures, a field which has seen the development of stable standards and advanced toolboxes and software, no such standards and open tools exist for continuous photoplethysmogram (PPG) analysis. Consequently, the primary objective of this research was to identify, standardize, implement and validate key digital PPG biomarkers. This work describes the creation of a standard Python toolbox, denoted pyPPG, for long-term continuous PPG time series analysis recorded using a standard finger-based transmission pulse oximeter. The improved PPG peak detector had an F1-score of 88.19% for the state-of-the-art benchmark when evaluated on 2,054 adult polysomnography recordings totaling over 91 million reference beats. This algorithm outperformed the open-source original Matlab implementation by ~5% when benchmarked on a subset of 100 randomly selected MESA recordings. More than 3,000 fiducial points were manually annotated by two annotators in order to validate the fiducial points detector. The detector consistently demonstrated high performance, with a mean absolute error of less than 10 ms for all fiducial points. Based on these fiducial points, pyPPG engineers a set of 74 PPG biomarkers. Studying the PPG time series variability using pyPPG can enhance our understanding of the manifestations and etiology of diseases. This toolbox can also be used for biomarker engineering in training data-driven models. pyPPG is available on this http URL

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

url_pdf: 'https://arxiv.org/pdf/2309.13767.pdf'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: **P.H. Charlton** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
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
