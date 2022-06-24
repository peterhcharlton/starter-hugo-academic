---
title: PPG Beat Detection
summary: Algorithms to detect heartbeats in photoplethysmogram (PPG) signals
tags:
- signal processing
- photoplethysmography
- atrial fibrillation
date: "2022-01-18T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Source [P.H. Charlton](https://commons.wikimedia.org/wiki/File:Detecting_atrial_fibrillation_(AF)_from_the_photoplethysmogram_(PPG).svg) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/PeterHCharlton
url_code: "https://ppg-beats.readthedocs.io/"

---

## Overview
The aim of this project is to develop a high-performance algorithm to detect heartbeats in photoplethysmogram (PPG) signals - the signals measured by smartwatches and pulse oximeters.

## Background
Smart wearables such as smartwatches and wrist-worn fitness trackers use photoplethysmography to monitor heart rate and rhythm. They do so by using an optical sensor to measure the photoplethysmogram (PPG) signal, and then analysing this signal to obtain heart rate or rhythm. A key step in analysing the signal is to identify individual heartbeats in the signal. Several approaches have previously been proposed to identify heartbeats in the signal, although it is not yet clear how well they perform, and whether they perform sufficiently well for clinical use.

## Aim
The aim of this project is to identify, or develop, a high-performance algorithm to detect heartbeats in photoplethysmogram (PPG) signals.

## Methods
The performance of existing PPG beat detection algorithms was assessed in different use cases, when using the algorithms with clinical monitoring data, and also wearable data. In addition, the impact of patient demographics and physiology was also assessed.

## Results
The results are currently under review in [this publication](./publication/assess_ppg_beat_detectors).

## Resources
The study is accompanied by the following resources, which are being made available [here](https://ppg-beats.readthedocs.io/):
1. **[PPG Beat Detection Algorithms](https://ppg-beats.readthedocs.io/en/latest/toolbox/ppg_beat_detectors)**: A selection of open-source algorithms for detecting beats in PPG signals.
2. **[Performance Assessment Resources](https://ppg-beats.readthedocs.io/en/latest/toolbox/performance_assessment)**: Resources to assess the performance of PPG beat detectors, including:
    - **[Datasets](https://ppg-beats.readthedocs.io/en/latest/datasets/summary)**: several publicly available datasets containing PPG and reference electrocardiogram (ECG) signals.
    - **[Code](https://ppg-beats.readthedocs.io/en/latest/toolbox/performance_assessment)**: MATLAB code with which to assess performance.
3. **[Tutorials](https://ppg-beats.readthedocs.io/en/latest/tutorials/summary)** on how to use the algorithms, datasets, and code.

## Status
The project is ongoing. Both this page and the accompanying resources will be updated further as the project progresses.
