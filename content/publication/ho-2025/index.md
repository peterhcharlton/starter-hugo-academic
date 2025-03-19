---
title: "Accurate RR-interval extraction from single-lead, telehealth electrocardiogram signals"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Sharon Yuen Shan Ho
- Florian Kristof
- Jonathan Mant
- admin

date: "2025-03-19T00:00:00Z"
doi: ""

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

abstract: Devices that record single-lead ECGs, such as smartwatches and handheld ECG recorders, hold promise for detecting undiagnosed atrial fibrillation (AF). Accurately extracting RR-intervals from telehealth ECGs is key for heart rhythm assessment. The aim of this study was to develop an algorithm to extract RR-intervals from telehealth ECGs, and assess whether the extracted RR-intervals are accurate and therefore suitable for analysis. Two datasets of 30-second handheld ECGs were used&#58; TELE ECG Database (250 ECGs) and SAFER ECG dataset (479 ECGs). One of three highperformance primary QRS detectors, selected based on previous evidence, was used to detect QRS complexes and extract RR-intervals. These detections were compared to those from a secondary QRS detector to assess accuracy. All pairs of 3 primary and 18 secondary QRS detectors were tested. Accuracy was quantified using mean absolute error (MAE) and the proportion of time RR-intervals were assessed as accurate (coverage). Best performance was achieved using unsw and nk as primary and secondary detectors, with MAEs of 24.6ms and 22.9ms, and coverages of 89% on TELE and SAFER respectively. Using a single detector alone produced higher MAEs (28.9ms and 48.0ms on TELE; 44.8ms and 48.4ms on SAFER). Accuracy was lower in AF (19.1 vs. 9.5ms, p<0.001) and low-quality signals (54.6 vs. 9.5ms, p<0.001). In conclusion, the recommended algorithm produced more accurate RR-intervals than using a single QRS detector, although accuracy was reduced in AF and low-quality signals.

# Summary. An optional shortened abstract.
summary: Using a pair of QRS detectors to determine when RR-intervals can be accurately extracted from ECGs

tags:
- electrocardiography

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Preprint
  url: https://doi.org/10.1101/2025.03.10.25323655

url_pdf: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: **S. Ho et al.** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
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

