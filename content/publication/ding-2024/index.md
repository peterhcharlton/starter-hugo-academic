---
title: "Comparing RR-Interval-Based and Whole-Signal-Based Machine Learning Models for Atrial Fibrillation Detection from Single-lead Electrocardiograms"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Zixuan Ding
- Jonathan Mant
- James Brimicombe
- Tommaso Bucci
- Benjamin JR Buckley
- Peter Calvert
- Wern Yew Ding
- Andrew Dymond
- Gregory Lip
- Riccardo Proietti
- Kate Williams
- Elena Punskaya
- admin

date: "2024-09-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *[CinC 2024](https://www.cinc2024.org/program/whova-program)*
publication_short: In *CinC 2024*

abstract: Single-lead ECGs can now be captured outside clinical environments, providing opportunities to detect atrial fibrillation (AF) in the general population. However, they can be of lower quality than 12-lead ECGs, which may result in features such as P-waves being obscured. This study aimed to compare the performance of machine learning models to detect AF from single-lead ECGs which use either RR-intervals alone or the entire ECG signal. Experiments were conducted using single-lead, 30-second ECG signals acquired using handheld ECG recorders, which are provided in two databases&#58; the Computing in Cardiology 2017 dataset (public), and the Screening for Atrial Fibrillation with ECG to Reduce Stroke (SAFER) dataset (private). The models assessed in this study were&#58; two models which used the entire ECG signal, both of which were top-performing models from the 2017 PhysioNet / Computing in Cardiology Challenge; and two RR-interval-based models - a state-of-the-art model and our proposed model which detects AF from a 2D representation of the differences between RR intervals. The performance of the models was evaluated separately on each dataset using the area under the Receiver-Operator Curve (AUROC) and Precision-Recall Curve (AUPRC). The models showed comparable AUROCs of 0.93 - 0.99. The AUPRCs varied more widely, from 0.64-0.94. Our proposed RR-interval-based AF detection model achieved an AUPRC of 0.94 on the CinC 2017 dataset, outperforming the state-of-the-art RR-interval-based model(0.88) and the entire-signal-based models (0.68 and 0.64). However, two of the state-of-the-art models performed better on the SAFER database (AUPRC of 0.75 for the RR-interval-based method, and 0.66 and 0.79 for entire-signal-based models) compared to our proposed model (0.71). This experiment demonstrated that AF detection models utilizing only RR intervals could achieve comparable performance to those utilizing the entire ECG signal. RR-interval-based models may have particular utility for analysing single-lead ECGs where features such as P-waves are obscured.

# Summary. An optional shortened abstract.
summary: Introducing two methods to benchmark the performance photoplethysmography (PPG) peak detectors.

tags:
- electrocardiography

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Preprint
  url: https://cinc.org/2024/Program/accepted/59_Preprint.pdf

url_pdf: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: **Z. Ding et al.** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
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

