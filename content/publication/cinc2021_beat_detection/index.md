---
title: "Benchmarking Photoplethysmography Peak Detection Algorithms Using the Electrocardiogram Signal as a Reference"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Kevin Kotzen
- admin
- Amir Landesberg
- Joachim A. Behar

date: "2021-09-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *[CinC 2021](https://www.cinc.org/2021/Program/accepted/PreliminaryProgram.html)*
publication_short: In *CinC 2021*

abstract: Photoplethysmography (PPG) is fast becoming the signal of choice for the widespread monitoring of sleep metrics obtained by wearable devices. Robust peak detection is critical for the extraction of meaningful features from the PPG waveform. There is however no consensus on what PPG peak detection algorithms perform best on nocturnal continuous PPG recordings. We introduce two methods to benchmark the performance PPG peak detectors. We make use of data where nocturnal PPG and electrocardiogram (ECG) are measured synchronously. Within this setting, the ECG, a signal for which there are established R-peak detectors, is used as reference. The first method for benchmarking, denoted 'Peak Matching', consists of forecasting the expected position of the PPG peaks using the ECG R-peaks as reference. The second technique, denoted 'IHR-IPR Accuracy', compares the instantaneous pulse rate (IPR) extracted from the PPG with the instantaneous heart rate (IHR) extracted from the ECG. For benchmarking, we used the MESA dataset consisting of 2,055 overnight polysomnography recordings with a combined length of over 16,300 hours. Four open PPG peak detectors were benchmarked. The 'Pulses' detector performed best with a Peak Matching F1-score of 0.94 and an IHR-IPR Accuracy of 89.6%. We introduced two new methods for benchmarking PPG peak detectors. Among the four detectors evaluated, 'Pulses' performed best. Benchmarking of further PPG detectors and on other data source (e.g. daytime recordings, recordings from patients with arrhythmia) is needed.

# Summary. An optional shortened abstract.
summary: Introducing two methods to benchmark the performance photoplethysmography (PPG) peak detectors.

tags:
- photoplethysmography
- wearables

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Preprint
  url: https://www.cinc.org/2021/Program/accepted/88_Preprint.pdf

url_pdf: ''

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
- SAFER Wearables

---

### Full text

- The published version will be available soon.

