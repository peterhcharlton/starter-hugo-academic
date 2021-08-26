---
title: "An impedance pneumography signal quality index: Design, assessment and application to respiratory rate monitoring"

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
- Jordi Alastruey

date: "2020-11-30T00:00:00Z"
doi: "10.1016/j.bspc.2020.102339"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Biomedical Signal Processing and Control*
publication_short: In *Biomed Signal Process Control*

abstract: Impedance pneumography (ImP) is widely used for respiratory rate (RR) monitoring. However, ImP-derived RRs can be imprecise. The aim of this study was to develop a signal quality index (SQI) for the ImP signal, and couple it with a RR algorithm, to improve RR monitoring. An SQI was designed which identifies candidate breaths and assesses signal quality using&#58; the variation in detected breath durations, how well peaks and troughs are defined, and the similarity of breath morphologies. The SQI categorises 32 s signal segments as either high or low quality. Its performance was evaluated using two critical care datasets. RRs were estimated from high-quality segments using a RR algorithm, and compared with reference RRs derived from manual annotations. The SQI had a sensitivity of 77.7%, and specificity of 82.3%. RRs estimated from segments classified as high quality were accurate and precise, with mean absolute errors of 0.21 and 0.40 breaths per minute (bpm) on the two datasets. Clinical monitor RRs were significantly less precise. The SQI classified 34.9% of real-world data as high quality. In conclusion, the proposed SQI accurately identifies high-quality segments, and RRs estimated from those segments are precise enough for clinical decision making. This SQI may improve RR monitoring in critical care. Further work should assess it with wearable sensor data.

# Summary. An optional shortened abstract.
summary: Design and assessment of a signal quality index for the impedance pneumography signal, and demonstration of its utility for respiratory rate monitoring.

tags: [impedance pneumography]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
links:
 - name: Submitted Manuscript
   url: https://zenodo.org/record/5211463/files/Impedance%20SQI%20manuscript%20-%20Oct%202020%20revision.docx?download=1

url_pdf: 'https://www.sciencedirect.com/science/article/pii/S1746809420304535/pdfft?md5=5e1d652e5a0ec73e95458825b143b0de&pid=1-s2.0-S1746809420304535-main.pdf'
url_code: 'https://doi.org/10.5281/zenodo.3973770'
url_dataset: 'https://doi.org/10.5281/zenodo.3973770'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Charlton PH et al. (CC BY 4.0)**](https://ars.els-cdn.com/content/image/1-s2.0-S1746809420304535-gr1.jpg)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- RRest

---
