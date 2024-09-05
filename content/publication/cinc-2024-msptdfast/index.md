---
title: "MSPTDfast - An Efficient Photoplethysmography Beat Detection Algorithm"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
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
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *[CinC 2024](https://www.cinc2024.org/program/whova-program)*
publication_short: In *CinC 2024*

abstract: Introduction&#58; Beat detection is a key step in the analysis of photoplethysmogram (PPG) signals. The MSPTD algorithm was recently identified as one of the most accurate beat detection algorithms, but its current open-source implementation is substantially more computationally expensive than other leading algorithms such as qppgfast. The aim of this work was to develop a more efficient, open-source implementation of the MSPTD algorithm. Methods&#58; Five potential improvements were identified to increase efficiency. Each potential improvement was evaluated in turn, and an optimal algorithm configuration named MSPTDfast was developed which incorporated all of the improvements found to reduce algorithm execution time whilst not substantially reducing the accuracy of beat detection. Performance was assessed using data collected from young adults during a lunchbreak in the PPG-DaLiA dataset. The data consisted of wrist PPG signals acquired using an Empatica E4 device, alongside simultaneous ECG signals from which reference heartbeat timings were obtained. Results&#58; MSPTDfast was found to be substantially more efficient than MSPTD (a reduction in execution time of 72.3%), with minimal difference in beat detection accuracy (F1-score 87.8% vs. 87.7%). In addition, the performance of MSPTDfast was much closer to that of the state-of-the-art qppgfast algorithm than the MSPTD algorithm, with a comparable F1-score (87.4% vs. 87.7%), and an execution time which was only 19.2% longer than that of qppgfast (vs. 330.8% longer for MSPTD). Conclusion&#58; In conclusion, MSPTDfast is an efficient and accurate open-source PPG beat detection algorithm with a substantially faster execution time than MSPTD. It is available under the permissive MIT licence.

# Summary. An optional shortened abstract.
summary: Developing a more efficient, open-source implementation of the MSPTD photoplethysmography beat detection algorithm

tags:
- photoplethysmography

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
- name: Preprint
  url: https://cinc.org/2024/Program/accepted/45_Preprint.pdf

url_pdf: ''

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