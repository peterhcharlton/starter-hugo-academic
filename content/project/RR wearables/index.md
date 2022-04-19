---
title: Respiratory rate algorithms for wearables
summary: Developing an algorithm to estimate respiratory rate from wearable photoplethysmogram (PPG) signals for use in daily life.
tags:
- wearables
- photoplethysmography
- respiratory rate
date: "2022-04-19T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Fitness tracker
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/PeterHCharlton
url_code: "https://github.com/peterhcharlton/RRest"
url_slides: "https://zenodo.org/record/4758898/files/RR%20algorithms%20for%20wearables%20intro.pdf?download=1"
url_video: "https://www.youtube.com/watch?v=C3JPImVkouc"

---

## Overview

The aim of the Respiratory Rate Estimation project is to develop and assess methods for automated respiratory rate (RR) monitoring. It consists of a series of studies of different algorithms for RR estimation from clinical data, complimented by the provision of publicly available datasets and resources.

## Background

Respiratory rate is a widely used indicator of health, used by clinicians in conjunction with other parameters to assess the health of patients in hospitals, clinics, and the community. For instance, all acutely-ill hospital patients have their respiratory rate measured every few hours to facilitate early detection of clinical deteriorations (deteriorations in health). However, respiratory rate is usually measured manually, by counting the number of breaths a patient takes in a specific period of time, such as a minute. This can potentially be time-consuming and inaccurate.

An alternative solution could be provided by developing an automated, electronic method for measuring respiratory rate using a device. To this end a plethora of algorithms have been proposed to estimate respiratory rate from several physiological signals, such as the electrocardiogram, photoplethysmogram, accelerometry signal, impedance pneumography signal, and so on. These signals can be easily measured, and in some scenarios are already measured for other purposes. Consequently, a robust, practicable algorithm for estimating respiratory rate from these signals could potentially benefit patients and healthcare providers alike.

## Methods

### Understanding the state-of-the-art
A [literature review](/publication/rr_review/) was conducted to understand the state-of-the-art on algorithms to estimate RR from the ECG and PPG. Briefly, we found that RR algorithms had been described in over 196 publications. We also found that previous studies assessing algorithm performance focused mostly on developing novel algorithms, rather than comparing algorithms. In addition, we found that the majority of previous studies of algorithm performance used data from young adults and healthy subjects, rather than assessing performance in our target setting of older, unhealthy adults.

This helped refine our research questions:
1. How well do respiratory rate algorithms perform in the target setting?
2. Which algorithm performs best?
3. Is it clinically useful?

### Developing a toolbox of algorithms

We implemented many of the RR algorithms described in the literature (which are now available in the [toolbox](#toolbox-of-rr-algorithms) detailed below). We verified their performance on ideal, simulated data in [this publication](/publication/rr_algs_assessment/).

### Assessment

The performance of RR algorithms was assessed on healthy volunteers in [this publication](/publication/rr_algs_assessment/), and on hospital patients in [this publication](/publication/cont_resp_monitoring/). Briefly, we found a wide variation in the performance of algorithms. Even the best algorithms can produce large errors, which would be clinically significant when compared to the normal RR range of 12-20 bpm.

The potential clinical utility of algorithms for detecting acute deteriorations in ambulatory hospital patients was assessed in [this publication](/publication/cont_resp_monitoring/).

### Future work

In the future, we would like to:
- Implement novel techniques designed to handle lower quality signals
- Assess the performance of algorithms in daily life
- Perform a comprehensive evaluation of algorithm performance across different settings

## Results

Please see the publications below for results arising from the project.

## Introductory Video

[This video](https://www.youtube.com/watch?v=C3JPImVkouc) provides an introduction to the project.

## Toolbox of RR Algorithms

Research into respiratory rate algorithms has been hindered by a lack of open-source algorithms. Consequently, one aim of this project is to provide open-source algorithms to facilitate future research. As stated in the licence accompanying the source code, the algorithms are not intended to be fit for any purpose. Instead, they act as an platform from which researchers can develop algorithms.

The following resources are provided:
- [Algorithm Source Code](https://github.com/peterhcharlton/RRest/archive/master.zip): The latest version of the toolbox of algorithms.
- [User Manual](https://github.com/peterhcharlton/RRest/wiki): A helpful resource for new users of the toolbox.
- [Github Repository](https://github.com/peterhcharlton/RRest): A repository of all versions of the toolbox, past and present.