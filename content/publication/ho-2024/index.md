---
title: "Automated RR Interval Detection and Quality Assessment in Telehealth Electrocardiograms"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Sharon Yuen Shan Ho
- Florian Kristof
- Jonathan Mant
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

abstract: Introduction&#58; Atrial fibrillation, a common heart arrhythmia, often goes undiagnosed, increasing stroke risk. Mobile health devices like smartwatches and handheld ECG recorders which can record single-lead ECGs could be used to screen for atrial fibrillation. A key step in using these ECGs is to detect irregular rhythms from RR-intervals. We aimed to develop an algorithm to automatically&#58; (i) derive RR-intervals from ECGs; and (ii) predict whether they are accurate enough to inform diagnosis. Methods&#58; The publicly available TELE ECG Database was used, containing 250 ECGs recorded by patients at home using a handheld ECG device, alongside manual annotations of QRS complexes. An algorithm was designed to&#58; (i) detect QRS complexes using a high-performance, primary QRS detection algorithm; (ii) assess their reliability by deeming each one to be reliable if it was also detected by a secondary QRS detection algorithm; and (iii) calculate RR-intervals as time delays between consecutive QRS complexes. Algorithm performance was assessed when using each combination of three primary and 18 secondary open-source QRS detection algorithms. Results&#58; Two approaches were used to identify optimal algorithm configurations. First, we identified the algorithm which produced the lowest mean absolute error (MAE) in those RR-intervals deemed to be reliable. This used 'unsw' as primary and 'rpeak' as secondary detectors, achieving a MAE of 24ms with 33&#37; of the RR-intervals deemed to be reliable. Second, we identified the algorithm with the lowest MAE, whilst deeming at least 90&#37; of RR-intervals to be reliable. This used 'unsw' as primary and 'nk' as secondary detectors, achieving a MAE of 33ms and deeming 92&#37; of RR-intervals to be reliable. Conclusion&#58; The proposed algorithms accurately derive RR-intervals from telehealth ECGs. This approach could be a valuable part of a pipeline for automatically identifying ECGs which show an irregular heart rhythm and therefore warrant manual review. 

# Summary. An optional shortened abstract.
summary: Using a pair of QRS detectors to determine when RR-intervals can be accurately extracted from ECGs

tags:
- electrocardiography

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Preprint
  url: https://cinc.org/2024/Program/accepted/84_Preprint.pdf

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

