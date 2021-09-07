---
title: 'Transcript for: An Introduction to Pulse Wave Modelling'
summary: Here we describe how to add a page to your site.
date: "2018-06-28T00:00:00Z"

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

This transcript accompanies [this talk](/talk/introduction-to-modelling-arterial-pulse-waves/).

Some of the transcript content is reproduced from the [accompanying paper](/publication/simulating_pulse_waves/) under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

## Title Slide

Topic for today:
- Using modelling to simulate pulse waves for research and development.

Personal introduction:
- Biomedical engineer specialising in signal processing for wearables.
- Institutions
- Current interests, and interests in vascular ageing.

---

# Part 1

## An Introduction to Pulse Wave Modelling using a 1D Model

---

## Introduction

I've used modelling in [my research](/publication/simulating_pulse_waves/) to simulate pulse waves, to investigate how vascular age can be assessed from arterial pulse waves. I've found it a useful tool for:
1. **Understanding physiological mechanisms**: Investigating what physiological mechanisms cause the changes in pulse waves that occur with age.
2. **Designing algorithms**: Designing algorithms to assess vascular age, by developing them using data from simulated subjects across a wide range of ages, and a wide range of cardiovascular properties.
3. **Investigating algorithm performance**: Investigating which cardiovascular properties can affect algorithm performance.

In this session I'll provide a brief overview of how this particular model works, and then demonstrate its utility through case studies. I'll conclude with some thoughts on the limitations, benefits and opportunities of this type of modelling.

## Accompanying Resources

You may find it helpful to have the [slides](/slides/intro_to_pulse_wave_modelling_slides/) in front of you.

During the session I'll ask a few questions, which you can contribute to either verbally, or through the [online poll](https://app.sli.do/event/1zunclmb). Do feel free to interrupt at any point.

---

## 1D Modelling

The model that I have used in my work is summarised in the image below.

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420001.jpeg" caption="**The one-dimensional model of pulse wave propagation (A) and simulated pulse waves (B).** <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

### The Model

This 1D model simulates blood flow, starting with flow into the aorta, then through the major arteries, and finally into the microcirculation. It consists of three main parts:
1. **Aortic Inflow:** The flow from the left ventricle into the aorta is specified. It is defined by several parameters, as illustrated in the image.
2. **Arterial Network:** The larger arteries of the body are specified in the model. The arteries are assumed to be thin, deformable, cylindrical tubes. They have a specified length, luminal diameter, and wall properties (such as arterial stiffness).
3. **Vascular Beds:** The vascular beds are themselves modelled using 0D (Windkessel) models, each with a specified resistance and compliance.

## Simulated Pulse Waves

Pulse waves can be simulated at any of the large arteries, as shown below:

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420005.jpeg" caption="Pressure (P) and flow velocity (U), luminal area (A) and photoplethysmogram (PPG) pulse waves simulated at common measurements sites. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

This image shows the different types of waveforms which the model can simulate:
- **Blood pressure (P)**
- **Blood flow velocity (U):** The speed at which blood flows through an artery.
- **Luminal area (A):** The cross-sectional area of an artery.
- **Photoplethysmogram (PPG):** An optical measure of blood volume in a vascular bed, commonly measured by pulse oximeters and digital wearable devices (_e.g._ smartwatches and fitness trackers).

One of the benefits of this type of modelling is that it allows waveforms to be simulated at multiple sites, and, it also captures the pulse transit times between different sites.

## Model Limitations

**Poll Question:** [What are the limitations of the model?](https://app.sli.do/event/1zunclmb)

## Possible Limitations

<details>
  <summary>A few thoughts</summary>
  
  1. Periodic inflow, as opposed to normal heart rate variability
  2. Specified arterial properties, which may not be representative of a particular individual
  3. Not able to model venous flow
</details>

## Input Parameters

The model requires a plethora of 'input parameters' (_i.e._ 'settings'), such as the heart rate, stiffness of each artery, and systemic vascular resistance. Some of these parameters have a marked impact on the simulated pulse waves, whereas others have only a small impact. For instance, the image below shows how the variation of each of the following input parameters impacts the simulated carotid and radial waveforms:
- HR: heart rate
- SV: stroke volume
- LVET: left ventricular ejection time
- PFT: time of peak aortic flow
- RFV: reverse flow volume caused by aortic valve closure at the end of systole
- Length: the length of the ascending aorta
- Diam: the diameters of the largest arteries (aorta and carotid)
- PWV: pulse wave velocities
- MAP: mean blood pressure
- PVC: peripheral vascular compliance

## Changing Inputs

**Question:** Which parameters would be most interesting to change, and why?

**Question:** Which parameters are most relevant to vascular ageing?

## Changing Inputs (2)

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420003.jpeg" caption="**Pulse waves (PWs) for the 25-yr-old subject at the carotid artery (A) and the radial artery (B).** The waves shown are at baseline (black), and those obtained when increasing (blue) and decreasing (red) each parameter independently by 1 SD from its baseline value. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

- Discuss figure: which parameters strongly influence the waves, and which don't?

## Changing Inputs (3)

A set of input parameters suitable for simulating pulse waves for young adults was proposed by (amongst others) [Mynard and Smolich](http://link.springer.com/10.1007/s10439-015-1313-8). We extended this by proposing a range of parameters to simulate pulse waves for healthy subjects aged 25-75, exhibiting a range of cardiovascular properties. Our proposed ranges of parameters are shown below:

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420002.jpeg" caption="**Proposed parameters to model healthy ageing and normal variation in cardiovascular properties:** The mean (solid line) and SD (dashed lines indicating &#177;1 and &#177;2 SD) values are shown for each parameter. The positive and negative SD values for carotid-femoral pulse wave velocities (PWVs) are different to capture the positive skewness of this variable's distribution. The final wave speed plot shows the baseline wave speed as a function of diameter for each age. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

These ranges of parameters are based on a review of those reported in the literature.

### A set of Virtual Subjects 

We aimed to create a set of virtual subjects representative of a sample of healthy subjects aged 25-75 years old. To do so:
1. **Baseline subject at each age:** We created a baseline subject for each age (25 to 75, in 10 year intervals), using the mean value of each parameter at that age.
2. **Varying parameters at each age:** We then created an additional 728 virtual subjects at each age by varying each parameter by &#177;1 SD from the mean, and creating a subject with each possible combination of parameters. Only the six most influential parameters were varied (HR, SV, LVET, Diam, PWV, PVR).
3. **Database of simulated pulse waves:** We created a [database](https://peterhcharlton.github.io/pwdb/pwdb.html) of simulated pulse waves for 4,374 virtual subjects (consisting of 729 at each of the six age groups). The database and accompanying code are publicly available.

### Comparison with _in vivo_ Data

We verified this approach for simulating pulse waves for subjects of different ages by comparing the simulated pulse waves with _in vivo_ pulse waves, as shown below:

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420006.jpeg" caption="**A comparison between simulated and in vivo pulse wave (PW) shapes. Each pair of plots shows in vivo PWs on the left, and simulated PWs on the right. PWs are shown for different ages in each plot, offset and normalized. Legends indicate ages. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)). Some of the in vivo data were obtained from Fluck et al. (doi: [10.3389/fphys.2014.00049](https://doi.org/10.3389/fphys.2014.00049); [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/))_">}}

**Poll Question:** [How well did the model perform?](https://app.sli.do/event/1zunclmb)

### Thoughts on Performance

<details>
  <summary>A few thoughts</summary>
  
  1. Captured increase in amplitude of second systolic peaks with age in carotid, aortic root and radial pressure waveforms.
  2. Captured disappearance of second peak of finger PPG waveform with age.
  3. Nonetheless, some marked differences between _in vivo_ and simulated waveforms.
</details>

Further details of the verification of this approach are provided in the [accompanying article](https://peterhcharlton.github.io/publication/simulating_pulse_waves/).

---

# Part 2:

## Case Study: Assessing Arterial Stiffness from the Photoplethysmogram

---

### Digital Wearable Device

One of the limitations of some current techniques for assessing arterial stiffness is that they require specialist equipment and/or specialist operators. A potential alternative is to acquire pulse waves using consumer devices worn in daily life, such as smartwatches or fitness trackers (shown below).

{{< figure src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/dc/Max_Health_Band.jpg/640px-Max_Health_Band.jpg" caption="**A wrist-worn device which acquires pulse waves by photoplethysmography.** <br> _Source: PH Charlton, [Max-Health-Band](https://commons.wikimedia.org/wiki/Category:Files_by_Peter_H_Charlton#/media/File:Max_Health_Band.jpg), Wikimedia Commons ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

### The Photoplethysmogram (PPG)

Digital wearable devices typically use photoplethysmography to acquire pulse waves:

{{< figure src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Photoplethysmogram_signal_components.svg/640px-Photoplethysmogram_signal_components.svg.png" caption="**Simplified origins of the photoplethysmogram (PPG) signal: arterial blood, venous blood and other tissues.** <br> _Source: PH Charlton, [Photoplethysmogram signal components](https://commons.wikimedia.org/wiki/File:Photoplethysmogram_signal_components.svg), Wikimedia Commons ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

### Changes in PPG Pulse Wave Shape

Many approaches have been proposed to assess arterial stiffness from the photoplethysmogram (PPG) signal, based on the observation that the PPG pulse wave changes shape with age:

{{< figure src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Classes_of_photoplethysmogram_%28PPG%29_pulse_wave_shape.svg/640px-Classes_of_photoplethysmogram_%28PPG%29_pulse_wave_shape.svg.png" caption="**Classes of photoplethysmogram (PPG) pulse wave shape:** Examples of the four classes of pulse wave shape proposed by Dawber et al. Generally, the higher classes are associated with older adults. <br> _Source: PH Charlton, [Classes of photoplethysmogram (PPG) pulse wave shape](https://commons.wikimedia.org/wiki/File:Classes_of_photoplethysmogram_(PPG)_pulse_wave_shape.svg), Wikimedia Commons ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

### Assessing Arterial Stiffness

Methods for assessing arterial stiffness from the PPG mostly consist of two steps (as shown below):
1. Identifying fiducial points (left)
2. Extracting pulse wave features (right)

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420004.jpeg" caption="**Pulse wave analysis:** Illustrated for a simulated pressure wave at the radial artery. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

The following three indices were extracted from PPG pulse waves in this case study:
1. Reflection Index (RI, illustrated)
2. Stiffness Index (SI)
3. Modified Aging Index (AGImod)

These were calculated for each virtual subject, and then their correlation with the reference aortic PWV was assessed. In addition, we investigated the cardiovascular determinants of each index.

### Results

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420009.jpeg" caption="The correlation of photoplethysmogram (PPG)-derived pulse wave (PW) indexes with aortic pulse wave velocity (PWV; A), and their physiological determinants (B). Data derived for all virtual subjects are shown in black, whereas red indicates data from 45-yr-old subjects. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

Discuss:
- Overall performance across all ages
- Performance within an individual age group
- Influence of not only PWV, but other CV properties (note difference in influence of 'diam')

### Implications:
1. Clinical studies should investigate performance over a small age range as well as over the entire cohort to assess the potential utility of indexes for stratifying patients
2. Indexes can also be influenced by HR and SV, indicating that it may be beneficial to assess performance when these CV properties are varied _in vivo_.

### Questions

1. What would you think of using this technology to assess vascular age?
2. How might it compare to other technologies?
3. How could one assess the relative performance of such technologies?

### Next Steps

The WG3 PPG group currently has a paper under review titled:

_Assessing Vascular Age from the Photoplethysmogram: A Systematic Review from VascAgeNet_

---

# Part 3

## Case Study: Changes in Pulse Pressure Amplification with Age

---

### Pulse Pressure Amplification

$$\mathrm{Pulse \ Pressure \ Amplification} = \frac{\mathrm{brachial \ pulse \ pressure}}{\mathrm{aortic \ pulse \ pressure}}$$

**Questions:**
1. How does pulse pressure amplification change with age?
2. Why?

### Methods

In this case study, we investigated the determinants of changes in PPamp with age. To do so, we assessed the effects of age on early systolic amplification and late systolic aortic pressure augmentation, calculated using the aortic PP at P1 and P2, respectively.

### Results

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420008.jpeg" caption="The causes of changes in pulse pressure (PP) amplification (PPamp) with age. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

**Question:** In A and B: how does the pulse wave change shape with distance from the aortic root to the finger? How does this differ with age?

Discuss:

The profiles demonstrate that two mechanisms influence PPamp (PPamp / PPb/PPa; subscripts "a" and "b" indicate aortic and brachial, respectively):
1. The early systolic portion was amplified in both subjects, causing SBPb to be greater than SBPa and therefore PPamp > 1. 
2. Late systolic aortic pressure augmentation (the increase in pressure from P1a to P2a) was higher in older subjects, increasing PPa and decreasing PPamp.

The contributions of these mechanisms to PPamp for the whole database are illustrated in panel C. The amplification of the early systolic portion increased with age, as shown in red by PPb/(P1a > DBPa). In contrast, the increase in late systolic aortic pressure augmentation with age (in blue) caused a decrease in PPb/(P2a > DBPa) with age. The effect of aortic pressure augmentation outweighed that of early systolic amplification, meaning PPamp decreased substantially with age, in keeping with in vivo studies. 

Early systolic amplification was determined primarily by the diameter of the larger arteries, and late systolic aortic pressure augmentation was largely determined by PWV and LVET, as shown in panels D and E. Indeed, since PPamp was primarily determined by late systolic aortic pressure augmentation, it was largely determined by arterial stiffness (i.e., PWV) and LVET, as shown in panel F. The change in PPamp observed with age was primarily due to changes in aortic pressure wave morphology.

### Implications

The database can be used to gain insight into the CV determinants of mechanisms of blood flow.

---

# Part 4

## Potential studies using blood flow modelling

---

### Exploring potential studies

Think of a study in which pulse wave modelling could be useful.

Consider:
- Research question
- What would need to be simulated?
- Under what conditions?
- In which ways would the model need to be particularly accurate?

### Limitations

- Dependent on model accuracy
- Which in turn, is dependent on input parameters
- Often requires specialist knowledge to perform studies

### Benefits 

- Allows pulse waves to be simulated under different conditions
- Control of physiology
- Free of measurement error
- Potentially cheap, and doesn't require participant involvement

### Opportunities

- Preliminary pilot work in technology development
- Inform the design of _in vivo_ studies
- Understand the potential shortcomings of existing technologies
- Understand the mechanisms underlying haemodynamic observations

## Further Reading and Resources

See the following:
- [Accompanying article](https://peterhcharlton.github.io/publication/simulating_pulse_waves/)
- [Database](https://peterhcharlton.github.io/pwdb/pwdb.html)
- [User Manual](https://github.com/peterhcharlton/pwdb/wiki)
- [Code for case studies](https://github.com/peterhcharlton/pwdb/wiki/Case-Studies)

## Acknowledgment

None of this would have been possible without:
- [Dr Jordi Alastruey-Arimon](http://haemod.uk/members/ja), who provided the [model](http://haemod.uk/nektar) and supervision
- The British Heart Foundation, who funded the work
- COST Action CA18216 "Network for Research in Vascular Ageing" supported by COST (European Cooperation in Science and Technology)

