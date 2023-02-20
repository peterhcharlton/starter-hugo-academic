---
title: "SleepPPG-Net: a deep learning algorithm for robust sleep staging from continuous photoplethysmography"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Kevin Kotzen
- admin
- Sharon Salabi
- Lea Amar
- Amir Landesberg
- Joachim Behar

date: "2022-11-29T00:00:00Z"
doi: "10.1109/JBHI.2022.3225363"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: IEEE Journal of Biomedical and Health Informatics
publication_short: IEEE JBHI

abstract: Sleep staging is an essential component in the diagnosis of sleep disorders and management of sleep health. Sleep is traditionally measured in a clinical setting and requires a labor-intensive labeling process. We hypothesize that it is possible to perform automated robust 4-class sleep staging using the raw photoplethysmography (PPG) time series and modern advances in deep learning (DL). We used two publicly available sleep databases that included raw PPG recordings, totalling 2,374 patients and 23,055 hours of continuous data. We developed SleepPPG-Net, a DL model for 4-class sleep staging from the raw PPG time series. SleepPPG-Net was trained end-to-end and consists of a residual convolutional network for automatic feature extraction and a temporal convolutional network to capture long-range contextual information. We benchmarked the performance of SleepPPG-Net against models based on the best-reported state-of-the-art (SOTA) algorithms. When benchmarked on a held-out test set, SleepPPG-Net obtained a median Cohen's Kappa score of 0.75 against 0.69 for the best SOTA approach. SleepPPG-Net showed good generalization performance to an external database, obtaining a Kappa score of 0.74 after transfer learning. Overall, SleepPPG-Net provides new SOTA performance. In addition, performance is high enough to open the path to the development of wearables that meet the requirements for usage in clinical applications such as the diagnosis and monitoring of obstructive sleep apnea.

# Summary. An optional shortened abstract.
summary: Sleep staging using photoplethysmography and deep learning.

tags:
- photoplethysmography
- deep learning
- sleep

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Submitted manuscript
  url: https://doi.org/10.48550/arXiv.2202.05735

url_pdf: '/publication/kotzen-2022/2022_Kotzen_et_al'

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

---

