---
title: "Machine learning-based pulse wave analysis for classification of circle of Willis topology - An in silico study with 30,618 virtual subjects"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Ahmet Sen
- Miquel Aguirre
- admin
- Laurent Navarro
- Stephane Avril
- Jordi Alastruey

date: "2025-02-01T00:00:00Z"
doi: "10.1016/j.bspc.2024.106999"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: Biomedical Signal Processing and Control
publication_short: BSPC

abstract: Background and Objective&#58; The topology of the circle of Willis (CoW) is crucial in cerebral circulation and significantly impacts patient management. Incomplete CoW structures increase stroke risk and post-stroke damage. Current detection methods using computed tomography and magnetic resonance scans are often invasive, time-consuming, and costly. This study investigated the use of machine learning (ML) to classify CoW topology through arterial blood flow velocity pulse waves (PWs), which can be noninvasively measured with Doppler ultrasound. Methods&#58; A database of in silico PWs from 30,618 virtual subjects, aged 25 to 75 years, with complete and incomplete CoW topologies was created and validated against in vivo data. Seven ML architectures were trained and tested using 45 combinations of carotid, vertebral and brachial artery PWs, with varying levels of artificial noise to mimic real-world measurement errors. SHapley Additive exPlanations (SHAP) were used to interpret the predictions made by the artificial neural network (ANN) models. Results&#58; A convolutional neural network achieved the highest accuracy (98%) for CoW topology classification using a combination of one vertebral and one common carotid velocity PW without noise. Under a 20% noise-to-signal ratio, a multi-layer perceptron model had the highest prediction rate (79%). All ML models performed best for topologies lacking posterior communication arteries. Mean and peak systolic velocities were identified as key features influencing ANN predictions. Conclusions&#58; ML-based PW analysis shows significant potential for efficient, noninvasive CoW topology detection via Doppler ultrasound. The dataset, post-processing tools, and ML code, are freely available to support further research.

# Summary. An optional shortened abstract.
summary: Using machine learning models to classify Circle of Willis topology based on carotid and vertebral flow velocity PWs.

tags:
- pwdb
- vascular ageing

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
#- name: Preprint
#  url: https://doi.org/10.1101/2024.08.23.24312514

url_pdf: 'https://www.sciencedirect.com/science/article/pii/S1746809424010577/pdfft'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: '[A. Sen et al.](#) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- vascular ageing

---
