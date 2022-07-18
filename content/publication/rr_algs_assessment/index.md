---
title: "An assessment of algorithms to estimate respiratory rate from the electrocardiogram and photoplethysmogram"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Timothy Bonnici
- Lionel Tarassenko
- David Clifton
- Richard Beale
- Peter Watkinson

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2016-03-30T00:00:00Z"
doi: "10.1088/0967-3334/37/4/610"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Physiological Measurement*
publication_short: In *Phys Meas*

abstract: Over 100 algorithms have been proposed to estimate respiratory rate (RR) from the electrocardiogram (ECG) and photoplethysmogram (PPG). As they have never been compared systematically it is unclear which algorithm performs the best. Our primary aim was to determine how closely algorithms agreed with a gold standard RR measure when operating under ideal conditions. Secondary aims were&#58; (i) to compare algorithm performance with IP, the clinical standard for continuous respiratory rate measurement in spontaneously breathing patients; (ii) to compare algorithm performance when using ECG and PPG; and (iii) to provide a toolbox of algorithms and data to allow future researchers to conduct reproducible comparisons of algorithms. Algorithms were divided into three stages&#58; extraction of respiratory signals, estimation of RR, and fusion of estimates. Several interchangeable techniques were implemented for each stage. Algorithms were assembled using all possible combinations of techniques, many of which were novel. After verification on simulated data, algorithms were tested on data from healthy participants. RRs derived from ECG, PPG and IP were compared to reference RRs obtained using a nasal-oral pressure sensor using the limits of agreement (LOA) technique. 314 algorithms were assessed. Of these, 270 could operate on either ECG or PPG, and 44 on only ECG. The best algorithm had LOAs of -4.7 to 4.7 bpm and a bias of 0.0 bpm when using the ECG, and -5.1 to 7.2 bpm and 1.0 bpm when using PPG. IP had LOAs of -5.6 to 5.2 bpm and a bias of -0.2 bpm. Four algorithms operating on ECG performed better than IP. All high-performing algorithms consisted of novel combinations of time domain RR estimation and modulation fusion techniques. Algorithms performed better when using ECG than PPG. The toolbox of algorithms and data used in this study are publicly available.

# Summary. An optional shortened abstract.
summary: An assessment of signal processing algorithms to estimate respiratory rate from signals typically acquired by wearables.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://iopscience.iop.org/article/10.1088/0967-3334/37/4/610/pdf'
url_code: 'https://github.com/peterhcharlton/RRest/tree/master/RRest_v2.0'
url_dataset: 'http://peterhcharlton.github.io/RRest/vortal_dataset.html'
url_slides: 'https://zenodo.org/record/166525/files/An%20Assessment%20of%20algorithms.pdf?download=1'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://cfn-live-content-bucket-iop-org.s3.amazonaws.com/journals/0967-3334/37/4/610/1/pmeaaa1942f01_hr.jpg?AWSAccessKeyId=AKIAYDKQL6LTV7YY2HIK&Expires=1624357814&Signature=iBmRO5HZf4DVRJrSDkdOqXNB%2BaM%3D)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- RRest
- RR wearables

---

### Prize

Awarded the [Martin Black Prize](https://iopscience.iop.org/journal/0967-3334/page/Martin_Black_award) for the best paper published in _Physiological Measurement_ in 2016.
