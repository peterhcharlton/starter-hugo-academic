---
title: "QRS detection in single-lead, telehealth electrocardiogram signals: benchmarking open-source algorithms
"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Florian Kristof
- Maximilian Kapsecker
- Leon Nissen
- James Brimicombe
- Martin Cowie
- Zixuan Ding
- Andrew Dymond
- Stephan Jonas
- Hannah Clair Linden
- Gregory Lip
- Kate Williams
- Jonathan Mant
- admin

date: "2023-11-08T00:00:00Z"
doi: "10.1101/2023.11.07.23298202"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: medRxiv
publication_short: medRxiv

abstract: Background and Objectives&#58; A key step in electrocardiogram (ECG) analysis is the detection of QRS complexes, particularly for arrhythmia detection. Telehealth ECGs present a new challenge for automated analysis as they are noisier than traditional clinical ECGs. The aim of this study was to identify the best-performing open-source QRS detector for use with telehealth ECGs. Methods&#58; The performance of 16 open-source QRS detectors was assessed on six datasets. These included four datasets of ECGs collected under supervision, and two datasets of telehealth ECGs collected without clinical supervision. The telehealth ECGs, consisting of single-lead ECGs recorded between the hands, included a novel dataset of 479 ECGs collected in the SAFER study of screening for atrial fibrillation (AF). Performance was assessed against manual annotations. Results&#58; A total of 12 QRS detectors performed well on ECGs collected under clinical supervision (F1 score >= 0.96). However, fewer performed well on telehealth ECGs&#58; five performed well on the TELE ECG Database (F1 of >= 0.99); four performed well on high-quality SAFER data (F1 of >= 0.96); and performance was poorer on low-quality SAFER data (three QRS detectors achieved F1 of 0.85-0.88). The presence of AF had little impact on performance. Conclusions&#58; The Neurokit, `two average', and University of New South Wales QRS detectors performed best in this study. These performed sufficiently well on high-quality telehealth ECGs, but not on low-quality ECGs. This demonstrates the need to handle low-quality ECGs appropriately to ensure only ECGs which can be accurately analysed are used for clinical decision making.

# Summary. An optional shortened abstract.
summary: An assessment of sixteen open-source QRS detection algorithms across six datasets.

tags:
- electrocardiogram
- wearables
- beat detection

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:

url_pdf: 'https://www.medrxiv.org/content/10.1101/2023.11.07.23298202v1.full.pdf'
url_code: 'https://github.com/floriankri/ecg_detector_assessment'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: **[P.H. Charlton et al.](https://iopscience.iop.org/article/10.1088/1361-6579/ac826d)** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- screening af

---

---

## Accompanying Resources

The code used in this study is available [here](https://github.com/floriankri/ecg_detector_assessment), including QRS detectors and the evaluation framework.

---

## Reproducing the analysis

The analysis reported in this study can be reproduced by following the steps [here](https://github.com/floriankri/ecg_detector_assessment/blob/publication/README.md).

---