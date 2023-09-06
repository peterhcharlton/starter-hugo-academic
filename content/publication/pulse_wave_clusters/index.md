---
title: "Clustered photoplethysmogram pulse wave shapes and their associations with clinical data"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Serena Zanelli
- Kornelia Eveilleau
- admin
- Mehdi Ammi
- Magid Hallab
- Mounim A. EL Yacoubi

date: "2023-09-05T00:00:00Z"
doi: "10.3389/fphys.2023.1176753"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Frontiers in Physiology*
publication_short: In *Front Physiol.*

abstract: Photopletysmography (PPG) is a non-invasive and well known technology that enables the recording of the digital volume pulse (DVP). Although PPG is largely employed in research, several aspects remain unknown. One of these is represented by the lack of information about how many waveform classes best express the variability in shape. In the literature, it is common to classify DVPs into four classes based on the dicrotic notch position. However, when working with real data, labelling waveforms with one of these four classes is no longer straightforward and may be challenging. The correct identification of the DVP shape could enhance the precision and the reliability of the extracted bio markers. In this work we proposed unsupervised machine learning and deep learning approaches to overcome the data labelling limitations. Concretely we performed a K-medoids based clustering that takes as input (i) DVP handcrafted features, (ii) similarity matrix computed with the Derivative Dynamic Time Warping and (iii) DVP features extracted from a CNN AutoEncoder. All the cited methods have been tested first by imposing four medoids representative of the Dawber classes, and after by automatically searching four clusters. We then searched the optimal number of clusters for each method using silhouette score, the prediction strength and inertia. To validate the proposed approaches we analyse the dissimilarities in the clinical data related to obtained clusters.

# Summary. An optional shortened abstract.
summary: Clustering photoplethysmogram pulse wave shapes and investigating clinical characteristics of different clusters.

tags: [photoplethysmography, pulse wave, machine learning]

# Display this page in the Featured widget?
featured: true

url_pdf: ''
url_code: ''
url_dataset: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Charlton PH et al. (CC BY 3.0)**](https://iopscience.iop.org/article/10.1088/1361-6579/aabe6a#pmeaaabe6af02)'
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

