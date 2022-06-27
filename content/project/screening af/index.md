---
title: Screening for atrial fibrillation
summary: Optimising screening for atrial fibrillation
tags:
- photoplethysmography
- atrial fibrillation
- electrocardiography
date: "2022-06-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Source - [OpenClipart-Vectors](https://pixabay.com/users/openclipart-vectors-30363/) from [Pixabay](https://pixabay.com/vectors/ekg-heartbeat-frequency-pulse-158177/) (Pixabay License)
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/PeterHCharlton

---

## Overview

In this project we are using signal processing and machine learning techniques to develop strategies to screen for atrial fibrillation (AF) which are both effective (ensuring patients with AF are correctly identified), and cost-effective (minimising the clinical workload involved in screening).

A commonly used approach to screen for AF consists of asking subjects to use a handheld electrocardiogram (ECG) recorder to record a single-lead ECG for 30 seconds. Typically, they are asked to do this several times a day for several weeks, so that even infrequent paroxysmal AF episodes can be identified. This approach is being used in the [SAFER Trial](https://www.safer.phpc.cam.ac.uk/).
   {{< figure src=/publication/reviewing_ecgs/featured.png caption="**Zenicor-EKG device and recorded ECGs**: A handheld device for recording single-lead ECGs. _Source: [Pandiaraja M. _et al._](https://doi.org/10.3390/ecsa-7-08195), [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)_">}}
   
Alternative approaches to screen for AF using wearables are being explored in the [SAFER Wearables Study](/project/safer-wearables).

## Background

Atrial fibrillation (AF) is a heart arrhythmia which is associated with a fivefold increase in risk of stroke, and yet is undiagnosed in 425,000 people in England. We are investigating whether screening for AF could reduce the incidence of stroke in the [SAFER Trial](https://www.safer.phpc.cam.ac.uk/). During screening, patients use a handheld device to record their electrocardiogram (ECG) four times a day for three weeks. This results in a large number of ECG recordings, and it isn't feasible to send all the ECGs for clinical review, as this would be highly costly and time-consuming. Therefore, there is a need to optimise strategies to screen for AF to ensure that subjects with AF are correctly identified, whilst minimising the number of ECGs sent for review.

## Aim

The aim of this project is to optimise strategies to screen for atrial fibrillation.

## Methods

We are using both in-house data and publicly available data to design ECG signal processing algorithms which extract parameters such as inter-beat intervals from ECGs. We are using real-world screening data (from the SAFER Trial) to develop strategies to identify ECGs which exhibit possible AF, and therefore require clinical review. We are using the same data to investigate the effectiveness and cost-effectiveness of such strategies.

## Results

Work is ongoing towards the following objectives:

### 1. Selecting ECGs for review

_Objective:_ To determine how best to select which ECGs should be clinically reviewed, using existing ECG analysis algorithms and novel approaches.

_Progress:_ To date, we have published on the potential benefits of excluding low quality ECGs from the review process in [this publication](/publication/reviewing_ecgs/). Work is ongoing to determine how best to select which ECGs out of the remainder to send for review. We are currently assessing how best to use existing ECG analysis algorithms to select which ECGs to review, aiming to send as few ECGs for review as possible (to minimise reviewing workload) whilst maintaining a high sensitivity to ECGs exhibiting AF. We are also comparing the characteristics of ECGs in AF and normal sinus rhythm to understand how algorithms could best discriminate between these two states.

### 2. Prioritising ECGs for review

_Objective:_ To develop a model to prioritise ECGs for review based on their probability of exhibiting AF, using signal processing and machine learning.

_Progress:_ To date, we have developed a simple model which uses RR-intervals to estimate the probability of an ECG containing AF (in [this publication](/publication/prioritising_ecgs/)). Metrics describing RR-intervals (such as their mean and standard deviation) were used as inputs to a logistic regression model, which outputted a probability of AF. Work is ongoing to incorporate additional inputs to the model, and to use more complex modelling methodology.

### 3. Visualising ECGs for review

_Objective:_ To develop visualisation techniques to aid ECG interpretation using explainable artificial intelligence.

_Progress:_ This will be a key task in [this PhD](/post/wd_armstrong_funding/). Briefly, we will examine different techniques for filtering ECGs to eliminate noise whilst maintaining physiological content, and we will look at approaches for annotating ECGs to explain to reviewers why they have been sent for review.

### 4. Optimising the manual review process

_Objective:_ To optimise the process for manually reviewing ECGs.

_Progress:_ Different approaches for manually reviewing ECGs were investigated in [this publication](/publication/reviewing_ecgs/), including the impact on workload of sending ECGs for review by one or two cardiologists. Ongoing work is further investigating the benefits and disadvantages of sending ECGs for review by multiple cardiologists. We are also aiming to develop tools to help train new reviewers of single-lead ECGs.



























