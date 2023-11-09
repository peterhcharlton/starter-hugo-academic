---
title: "Robust peak detection for photoplethysmography signal analysis"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Marton A. Goda
- admin
- Joachim A. Behar

date: "2023-07-18T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: In *[CinC 2023](https://cinc.org/prelim_program_2023/)*
publication_short: In *CinC 2023*

abstract: Efficient and accurate evaluation of long-term photoplethysmography (PPG) recordings is essential for both clinical assessments and consumer products. In 2021, the top opensource peak detectors were benchmarked on the Multi-Ethnic Study of Atherosclerosis (MESA) database consisting of polysomnography (PSG) recordings and continuous sleep PPG data, where the Automatic Beat Detector (Aboy) had the best accuracy. This work presents Aboy++, an improved version of the original Aboy beat detector. The algorithm was evaluated on 100 adult PPG recordings from the MESA database, which contains more than 4.25 million reference beats. Aboy++ achieved an F1-score of 85.5%, compared to 80.99% for the original Aboy peak detector. On average, Aboy++ processed a 1 hour-long recording in less than 2 seconds. This is compared to 115 seconds (i.e., over 57-times longer) for the open-source implementation of the original Aboy peak detector. This study demonstrated the importance of developing robust algorithms like Aboy++ to improve PPG data analysis and clinical outcomes. Overall, Aboy++ is a reliable tool for evaluating long-term wearable PPG measurements in clinical and consumer contexts.

# Summary. An optional shortened abstract.
summary: A high-performance beat detector for the photoplethysmogram signal.

tags:
- photoplethysmogram
- signal processing

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Preprint
  url: https://arxiv.org/pdf/2307.10398.pdf

url_pdf: 'https://arxiv.org/pdf/2307.10398.pdf'

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
- ppg-beats

---

