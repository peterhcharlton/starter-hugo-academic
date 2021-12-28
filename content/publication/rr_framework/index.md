---
title: "A new framework to estimate breathing rate from electrocardiogram, photoplethysmogram, and blood pressure signals"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Ali Adami
- Reza Boostani
- Faezeh Marzbanrad
- admin

date: "2021-03-17T00:00:00Z"
doi: "10.1109/ACCESS.2021.3066166"

# Schedule page publish date (NOT publication's date).
publishDate: "2021-10-10T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *IEEE Access*
publication_short: In *IEEE Access*

abstract: Breathing Rate (BR) is a key physiological parameter measured in a wide range of clinical settings. However, it is still widely measured manually. In this paper, a novel framework is proposed to estimate the BR from an electrocardiogram (ECG), a photoplethysmogram (PPG), or a blood pressure (BP) signal. The framework uses Empirical Mode Decomposition (EMD) and Discrete Wavelet Transform (DWT) methods to extract respiratory signals, taking advantage of both time and frequency domain information. An Extended Kalman Filter (EKF), incorporating a Signal Quality Index (SQI), enabled our method to achieve acceptable performance even for significantly distorted periods of the signals. Using state vector fusion, the output signals are combined and finally the BR is estimated. The framework was tested on two publicly available clinical databases&#58; the MIT-BIH Polysomnographic and BIDMC databases. Performance was evaluated using the mean absolute percentage error (MAPE). The results indicated high accuracy&#58; MAPEs on the two databases of 3.9% and 3.6% for ECG signals, 6.0% for PPG, and 5.0% for BP signals. The results also indicated high robustness to noise down to 0dB. Therefore, this framework may have utility for BR monitoring in high noise settings.

# Summary. An optional shortened abstract.
summary: A novel method to estimate respiratory rate from non-invasive signals.

tags:
- photoplethysmography
- signal processing
- respiratory rate
- electrocardiogram

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:

url_pdf: 'https://ieeexplore.ieee.org/iel7/6287639/9312710/09380434.pdf'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Source: **[A. Adami _et al._](https://doi.org/10.1109/ACCESS.2021.3066166)** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- Respiratory rate algorithms for wearables
---

