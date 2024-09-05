---
title: "The MSPTDfast photoplethysmography beat detection algorithm - Design, benchmarking, and open-source distribution"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Erick Javier Arguello-Prada
- Jonathan Mant
- Panicos A. Kyriacou

date: "2024-09-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: Under review
publication_short: Under review

abstract: Objective&#58; Photoplethysmography is widely used for physiological monitoring, whether in clinical devices such as pulse oximeters, or consumer devices such as smart-watches. A key step in the analysis of photoplethysmogram (PPG) signals is detecting heartbeats. The MSPTD algorithm has been found to be one of the most accurate PPG beat detection algorithms, but is less computationally efficient than other algorithms. Therefore, the aim of this study was to develop a more efficient, open-source implementation of the MSPTD algorithm for PPG beat detection, named MSPTDfast (v.2). Approach&#58; Five potential improvements to MSPTD were identified and evaluated on four datasets. MSPTDfast (v.2) was designed by incorporating each improvement which on its own reduced execution time whilst maintaining a high F1-score. After internal validation, MSPTDfast (v.2) was benchmarked against state-of-the-art beat detection algorithms on four additional datasets. Main results&#58; MSPTDfast (v.2) incorporated two key improvements&#58; pre-processing PPG signals to reduce the sampling frequency to 20 Hz; and only calculating scalogram scales corresponding to heart rates >30 bpm. During internal validation MSPTDfast (v.2) was found to have an execution time of between approximately one-third and one-twentieth of MSPTD, and a comparable F1-score. During benchmarking MSPTDfast (v.2) was found to have the highest F1-score alongside MSPTD, and amongst one of the lowest execution times with only MSPTDfast (v.1), qppgfast and MMPD (v.2) achieving shorter execution times. Significance&#58; MSPTDfast (v.2) is an accurate and efficient PPG beat detection algorithm, available in an open-source Matlab toolbox.

# Summary. An optional shortened abstract.
summary: Developing and benchmaking a more efficient, open-source implementation of the MSPTD photoplethysmography beat detection algorithm

tags:
- photoplethysmography

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Preprint
  url: https://doi.org/10.1101/2024.08.23.24312514

url_pdf: 'https://www.medrxiv.org/content/10.1101/2024.08.23.24312514v1.full.pdf'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: '[P. Charlton et al.](#) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))'
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

### Accompanying presentation

The presentation which accompanies this paper is available [here](/talk/msptdfast-an-efficient-photoplethysmography-beat-detection-algorithm/).