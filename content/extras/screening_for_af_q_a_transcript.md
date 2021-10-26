---
title: 'Transcript for: Screening for AF - questions and potential answers'
summary: An update on the work of the SAFER Programme on screening for atrial fibrillation.
date: "2021-09-20T13:00:00Z"

reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: false  # Show comments?

# Optional header image (relative to `assets/media/` folder).
header:
  caption: ""
  image: ""
---

# Overview

This transcript accompanies [this talk](/talk/screening-for-af-questions-and-potential-answers/).

Some of the transcript content is reproduced from the [accompanying paper](/publication/reviewing_ecgs/) under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

## Title Slide

Topic for today:
- Screening for atrial fibrillation: questions and potential answers.

---

## Clinical Problem: undiagnosed AF

[Click] If atrial fibrillation was adequately treated in England, then it's estimated that this could save [click] 2,000 lives per year, [click] prevent 7,000 strokes, and result in an additional 425,000 diagnoses.

---

## Potential Solution: AF screening

It has been proposed that undiagnosed AF could be identified through screening. However, "it is unclear whether there is a benefit of formal screening programmes for AF over and above diagnosis of AF only through routine clinical practice" [[UK National Screening Committee, 2019](https://view-health-screening-recommendations.service.gov.uk/atrial-fibrillation/)]. The ongoing [SAFER Trial](https://www.safer.phpc.cam.ac.uk/) [click] aims to determine whether screening for AF is effective and cost-effective in reducing stroke.

---

## Personal Introduction

To introduce myself [click], my name's Peter Charlton, and I'm a researcher in Biomedical Engineering. I develop techniques to analyse physiological signals, such as the ECGs acquired in screening studies, to aid clinical decision making. I initially conducted my research here at St Thomas' Hospital in London, working with clinicians to develop techniques to identify the early signs of clinical deterioration from wearable sensor signals. Since then, I've been analysing ECG data [click] collected by the SAFER Research Team, at the University of Cambridge.

---

## Overview

In this talk I'll look at three key questions and potential answers:
1. Is screening for AF effective?
2. How can today's screening be optimised?
3. What might tomorrow's screening look like?

Firstly, an introduction to AF screening and the SAFER Programme.

---

## Atrial Fibrillation

AF is one of the most common arrhythmias, diagnosed in 3% of UK people over the age of 35 [[Adderley _et al._](https://doi.org/10.1136/heartjnl-2018-312977)]. It is associated with a fivefold increase in stroke risk [[Wolf _et al._](https://doi.org/0.1161/01.str.22.8.983)]. If AF is recognised then the risk of stroke can be reduced by 60-70% through anticoagulation [[Hart _et al._](http://www.ncbi.nlm.nih.gov/pubmed/17577005), [Yao _et al._](https://doi.org/10.1161/JAHA.116.003725)]. AF is currently diagnosed opportunistically in primary care, and verified by ECG. Whilst some cases of AF are persistent [click], meaning that the patient is in AF all the time, others are paroxysmal [click], meaning there are only intermittent episodes of AF which could be missed in a one-off ECG test. Furthermore, AF can be asymptomatic [click], meaning testing may not be indicated.

---

## The SAFER Programme

The SAFER Programme of research, led by Prof Jonathan Mant, aims to determine [click] whether screening for AF is effective and cost-effective in reducing stroke and other key outcomes compared to current practice. It consists of [click] four parts [[SAFER Website](https://www.safer.phpc.cam.ac.uk/about-screenforaf/aims-and-objectives/)]:

1. **Feasibility study 1:** A study in 10 GP Practices, including a face-to-face appointment, which 2,141 participants took part in. This has finished, confirming that it is feasible to deliver an AF screening programme in general practice, and that high numbers of patients accept an offer of AF screening and go on to complete the screening process.
2. **Feasibility study 2:** When the COVID-19 pandemic struck, it became clear that screening could not be delivered in the practice. An additional feasibility study was conducted with participants from 3 GP Practices, in which the screening was delivered remotely.
3. **Internal pilot study:** The first phase of the trial is now underway. An internal pilot study is being conducted in 36 practices, consisting of 12 intervention practices where patients will be offered screening, and 24 control practices.
4. **Cluster randomised controlled trial:** Following the pilot, we expect to move straight into the remainder of the trial, including a further 324 practices. The whole trial, including the internal pilot, will enrol approximately 126,000 patients from 360 practices, a third of whom will be offered screening. They will be followed up for an average of 5 years.

---

## The Screening Process

The three main steps of the screening process which I'll refer to are as follows [click]:

1. **ECGs recorded at home:** Firstly, participants are sent a handheld device which takes 30-second ECG recordings between two thumbs. Participants are asked to record an ECG 4 times per day, for 3 weeks [[SAFER Website](https://www.safer.phpc.cam.ac.uk/for-patients/screening-process/)], producing approximately 84 ECGs per participant.
2. **Automated analysis:** Secondly, the ECG recordings are automatically analysed to identify any that may contain AF.
3. **Clinical review:** Thirdly, those ECGs which may contain AF are sent for clinical review to make a final diagnosis. Any participants diagnosed with AF then discuss possible anticoagulation with their GP.

---

## Is screening for AF effective?

So, the first question.

---

## Is screening for AF effective and cost effective in reducing stroke and other key outcomes compared to current practice?

This question hasn't yet been answered in the ongoing SAFER Trial. However, results were recently published for the STROKESTOP trial, a trial using the same handheld devices in Sweden [[ref](https://doi.org/10.1016/s0140-6736(21)01637-8)]. There was a "small net benefit" to screening, as shown by the significantly lower number of events in those invited to screening, compared to the control group. Although there were some differences in trial design, the trial does provide some useful learning points for SAFER, including:
- For screening to be effective, a high proportion of those invited to screening have to participate, since the endpoint was calculated using the intention-to-treat analysis, as is the case in SAFER. In STROKESTOP, of those invited to screening, 51.3% participated. Indeed, those who "declined the invitation for screening ... had higher ... stroke risk" [[Lowres _et al._](10.1016/s0140-6736(21)01750-5)]. As noted in the accompanying commentary, "A different approach is being adopted in the SAFER study, in which patients in general practices are invited to join the study, and practices are only randomly assigned to screening or control after a sufficient number of patients consent, which should obviate the design problem of dilution by non-participants" [[Lowres _et al._](10.1016/s0140-6736(21)01750-5)]. Qualitative researchers in the SAFER team are collecting feedback from non-participants to understand why people decline the invitation to screening.
- [click] The results also show promise for the choice of combined ischaemic and haemorrhagic stroke as the primary endpoint in SAFER. Both of these endpoints showed a signal towards a difference, although this was not significant difference.

---

## How can today's screening be optimised? (outline)

So, the second question: How can today's screening be optimised? My colleagues and I have been working on optimising the acquisition of ECGs, and their automated review. I'll present preliminary analyses on these two aspects.

---

## ECGs recorded at home

Firstly, [click] we are establishing criteria to prompt a telephone call from the research team to participants to provide additional training when required on taking ECGs.

[Click] Many of the ECGs collected in SAFER are of high quality, such as this ECG here. However, [click] some ECGs are of low quality. These are often difficult, if not impossible, to interpret. Consequently, if a participant records too many low quality ECGs then it may not be possible to accurately identify AF.

[Click] In a retrospective analysis of data from the first SAFER Feasibility Study, we investigated the performance of different criteria for identifying participants who would record a high proportion of low quality ECGs. The analysis was performed on 1,486 participants, who each recorded at least 56 ECGs. The criteria were applied to ECGs received during the first 10 days (i.e. the first half) of screening. We aimed for a high sensitivity to participants with less than 75% high quality ECGs, and a low alert rate to minimise the workload associated with the additional calls.

[Click] Here are the results for three candidate criteria. For each criterion, a threshold was learnt from the data. The third criterion, which consisted of triggering a call if more than 25% of a participant's ECGs were of low quality, resulted in a high sensitivity at the desired alert rate.

---

## Effectiveness of criterion to prompt a training call

[Click] The effectiveness of this criterion was then assessed when it was used in the second SAFER Feasibility Study. This study was smaller, with _n_ participants. _n_ of these participants received a telephone call - reassuringly, this indicates an alert rate of approximately 4% as desired. It's testament to the SAFER Team that these calls resulted in a reduction in the percentage of low quality recordings, as shown in this box plot. _(describe reduction shown in plot)_

So, we have found that training calls can be targeted to those participants who would benefit most from them, and that they are effective in improving the quality of ECG recordings.

---

## Automated analysis

A second analysis which informed the Trial's methodology was an assessment of the performance of algorithm tags for identifying AF, and the workload associated with reviewing ECGs classified with each tag.

I'll briefly summarise how the algorithm works. [Click] Each ECG is analysed by [click] detecting heartbeats, [click] analysing the heart rhythm, and assessing [click] whether P-waves are present or not. A key question [click] is: which tags should be used to identify ECGs for review?

[click] In a retrospective analysis, I assessed the sensitivity of each tag to AF, and its positive predictive value. This was performed using manual annotations of 911 ECGs containing AF provided by cardiologists. Six tags showed reasonable performance (shown in bold). These were considered as candidates to identify ECGs for clinical review.

[click] In a second analysis, I investigated the workload and effectiveness of the combination of tags used in this Feasibility Study, and all possible combinations of the candidate tags. The combination of tags used in the study, shown in the first row, was particularly comprehensive, and resulted in 23,000 ECGs being sent for review. Through this process 54 participants were diagnosed with AF. The remaining rows show selected combinations using subsets of these tags. As the number of tags is reduced, the number of ECGs sent for review is reduced. Only in the last combination, the irregular sequence tag on its own, was there an impact on the diagnosis of AF, with one participant being missed.

Based on this, I recommended that the irregular sequence and fast regular tags be used in SAFER, which in this analysis would have substantially reduced the workload associated with ECG reviewing, whilst maintaining the number of AF diagnoses.

---

## How can today's screening be optimised?

Today I've presented preliminary results on questions relating to optimising the current approach to screening, specifically on: training calls, and the automated analysis of ECGs. In addition, I am particularly interested in the following additional questions:
- Can ECGs be ordered according to their likelihood of exhibiting AF?
- What is the level of inter-reviewer agreement in diagnoses?
- How many reviewers should review each patient?s data?
- Can we develop a library of ECGs with which to train new reviewers?

---

## What might tomorrow's screening look like? (outline)

So, the third question: What might tomorrow's screening look like? As an engineer, it is my hope that the data collected in both the SAFER Programme and follow-on studies will be useful for informing tomorrow's approach to screening.

---

## Could consumer devices be used for clinical decision making?

A key question going forward will be: Could consumer devices be used for clinical decision making?

Devices like those shown here are commercially available, including the AliveCor device (left), which allows users to record their ECG with a small add-on to their smartphone. Watches by Withings [click], such as that shown here, also allow users to record a 30-second ECG. And, fitness trackers and smartwatches which measure the arterial pulse wave are now commonplace [click], some of which can identify an irregular pulse which may be indicative of AF. We are starting the SAFER Wearables study, a study to assess the acceptability and performance of wearables such as those shown here for identifying AF in older adults.

---

## Using consumer devices to identify AF

Indeed, it has already been shown that smartwatches could potentially be used to unobtrusively check for AF in daily life as follows. In [click] a normal rhythm, [click] the beat-to-beat intervals are fairly consistent. In contrast, [click] in atrial fibrillation the beat-to-beat intervals are irregular [click]. Potentially, a consumer wearable could be used to identify possible AF episodes in this manner. Indeed, the potential utility of an Apple Watch to identify AF was recently assessed in the Apple Heart Study in over 400,000 individuals. Key results included a reassuringly low alert rate [click], a high positive predictive value of alerts [click], and a much longer monitoring time [click] than could be achieved at scale in clinical practice. In this study, possible AF episodes prompted further monitoring using the gold standard of an ECG-based wearable in order to confirm a diagnosis.

The SAFER Wearables Study will add to this evidence by assessing the performance of the technology in older adults, and daily life - two aspects that in our opinion, require further investigation.

---

## Thanks

None of this would have been possible without:
- [Prof Jonathan Mant](https://www.phpc.cam.ac.uk/people/pcu-group/pcu-senior-academic-staff/jonathan-mant/), who leads the SAFER Programme.
- The [SAFER Research Team](https://www.safer.phpc.cam.ac.uk/about-us/research-team/)
- The NIHR and BHF, who funded the work

---

## Conclusions

To conclude:
- Evidence is emerging showing the clinical benefit of AF screening.
- Trials are ongoing, which will also assess the cost-effectiveness.
- If wearables are used to identify AF, they should be like a harness: highly reliable, and for a specified purpose.
