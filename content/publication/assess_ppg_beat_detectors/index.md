---
title: "Detecting beats in the photoplethysmogram: benchmarking open-source algorithms"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Kevin Kotzen
- Elisa Mejia-Mejia
- Philip J. Aston
- Karthik Budidha
- Jonathan Mant
- Callum Pettit
- Joachim Behar
- Panicos A. Kyriacou

date: "2022-07-18T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: Physiological Measurement
publication_short: Physiological Measurement

abstract: The photoplethysmogram (PPG) signal is widely used in pulse oximeters and smartwatches. A fundamental step in analysing the PPG is the detection of heartbeats. Several PPG beat detection algorithms have been proposed, although it is not clear which performs best. Objective&#58; This study aimed to&#58; (i) develop a framework with which to design and test PPG beat detectors; (ii) assess the performance of PPG beat detectors in different use cases; and (iii) investigate how their performance is affected by patient demographics and physiology. Approach&#58; Fifteen beat detectors were assessed against electrocardiogram-derived heartbeats using data from eight datasets. Performance was assessed using the F1 score, which combines sensitivity and positive predictive value. Main results&#58; Eight beat detectors performed well in the absence of movement with F1 scores of &ge;90% on hospital data and wearable data collected at rest. Their performance was poorer during exercise with F1 scores of 55-91%; poorer in neonates than adults with F1 scores of 84-96% in neonates compared to 98-99% in adults; and poorer in atrial fibrillation (AF) with F1 scores of 92-97% in AF compared to 99-100% in normal sinus rhythm. Significance&#58; Two PPG beat detectors denoted 'MSPTD' and 'qppg' performed best, with complementary performance characteristics. This evidence can be used to inform the choice of PPG beat detector algorithm. The algorithms, datasets, and assessment framework are freely available.

# Summary. An optional shortened abstract.
summary: An assessment of fifteen open-source photoplethysmogram (PPG) beat detectors across eight datasets.

tags:
- photoplethysmography
- wearables
- beat detection

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:

url_pdf: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: **P.H. Charlton et al.** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- ppg-beats

---

## Accompanying Resources

The ['ppg-beats'](https://ppg-beats.readthedocs.io/) toolbox of algorithms and code was used in this study.