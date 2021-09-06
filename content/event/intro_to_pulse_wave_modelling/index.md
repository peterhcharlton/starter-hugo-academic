---
title: Introduction to modelling arterial pulse waves

event: VascAgeNet [Training School](https://vascagenet.eu/training-schools)

location: Split, Croatia

summary: An introduction to modelling arterial pulse waves. 
abstract: In this training event I provided an introduction to modelling arterial pulse waves, summarising how arterial pulse waves can be simulated using a computational model of blood flow around the body. I then demonstrated the utility of such modelling in three case studies. Finally, I summarised the limitations of this type of modelling, its benefits, and opportunities for further research.


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2021-09-07T17:00:00Z"
date_end: "2021-09-07T19:30:00Z"
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: "2017-01-01T00:00:00Z"

authors: [admin]
tags: [vascular ageing, pulse waves, arterial stiffness, blood pressure, photoplethysmography]

# Is this a featured talk? (true/false)
featured: false

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/PeterHCharlton
- name: Event Poll
  url: https://app.sli.do/event/1zunclmb
- name: Accompanying Paper
  url: https://peterhcharlton.github.io/publication/simulating_pulse_waves/
- name: Pulse Wave Database
  url: https://peterhcharlton.github.io/pwdb/pwdb.html
url_code: "https://github.com/peterhcharlton/pwdb/wiki/Case-Studies"
url_pdf: ""
url_slides: ""
url_video: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
- Modelling arterial pulse waves
---

## Introduction

I've used modelling in [my research](/publication/simulating_pulse_waves/) to simulate pulse waves, to investigate how vascular age can be assessed from arterial pulse waves. I've found it a useful tool for:
1. **Understanding physiological mechanisms**: Investigating what physiological mechanisms cause the changes in pulse waves that occur with age.
2. **Designing algorithms**: Designing algorithms to assess vascular age, by developing them using data from simulated subjects across a wide range of ages, and a wide range of cardiovascular properties.
3. **Investigating algorithm performance**: Investigating which cardiovascular properties can affect algorithm performance.

In this session I'll provide a brief overview of how this particular model works, and then demonstrate its utility through three case studies. I'll conclude with some thoughts on the limitations, benefits and opportunities of this type of modelling.

During the session I'll ask a few questions, which you can contribute to either verbally, or through the [online poll](https://app.sli.do/event/1zunclmb). Do feel free to interrupt at any point.

## 1D Modelling

The model that I have used in my work is summarised in the image below.

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420001.jpeg" caption="**The one-dimensional model of pulse wave propagation (A) and simulated pulse waves (B).** <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

### The Model

The model simulates blood flow, starting with flow into the aorta, then through the major arteries, and finally into the microcirculation. It consists of three main parts:
1. **Aortic Inflow:** The flow from the left ventricle into the aorta is specified. It is defined by several parameters, as illustrated in the image.
2. **Arterial Network:** The larger arteries of the body are specified in the model. The arteries are assumed to be thin, deformable, cylindrical tubes. They have a specified length, luminal diameter, and wall properties (such as arterial stiffness).
3. **Vascular Beds:** The vascular beds are themselves modelled using 0D (Windkessel) models, each with a specified resistance and compliance.

### Simulated Waveforms

The image above shows the different types of waveforms which the model can simulate (see panel **B** of the image, on the right hand side):
- **Blood flow rate (denoted Q):** The rate at which blood flows through an artery.
- **Luminal area (A):** The cross-sectional area of an artery.
- **Blood flow velocity (U):** The speed at which blood flows through an artery.
- **Blood pressure (P)**
- **Photoplethysmogram (PPG):** An optical measure of blood volume in a vascular bed, commonly measured by pulse oximeters and digital wearable devices (_e.g._ smartwatches and fitness trackers).

### Limitations

**Poll Question:** [What are the limitations of the model?](https://app.sli.do/event/1zunclmb)

<details>
  <summary>A few thoughts</summary>
  
  1. Periodic inflow, as opposed to normal heart rate variability
  2. Specified arterial properties, which may not be representative of a particular individual
  3. Not able to model venous flow
</details>

### Specifying Model Input Parameters

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

**Question:** Which parameters would be most interesting to change, and why?

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420003.jpeg" caption="**Pulse waves (PWs) for the 25-yr-old subject at the carotid artery (A) and the radial artery (B).** The waves shown are at baseline (black), and those obtained when increasing (blue) and decreasing (red) each parameter independently by 1 SD from its baseline value. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

A set of input parameters suitable for simulating pulse waves for young adults was proposed by (amongst others) [Mynard and Smolich](http://link.springer.com/10.1007/s10439-015-1313-8). We extended this by proposing a range of parameters to simulate pulse waves for healthy subjects aged 25-75, exhibiting a range of cardiovascular properties. Our proposed ranges of parameters are shown below:

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420002.jpeg" caption="**Proposed parameters to model healthy ageing and normal variation in cardiovascular properties:** The mean (solid line) and SD (dashed lines indicating &#177;1 and &#177;2 SD) values are shown for each parameter. The positive and negative SD values for carotid-femoral pulse wave velocities (PWVs) are different to capture the positive skewness of this variable's distribution. The final wave speed plot shows the baseline wave speed as a function of diameter for each age. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))._">}}

These ranges of parameters are based on a review of those reported in the literature.

### Creating a set of Virtual Subjects 

We aimed to create a set of virtual subjects representative of a sample of healthy subjects aged 25-75 years old. To do so:
1. **Baseline subject at each age:** We created a baseline subject for each age (25 to 75, in 10 year intervals), using the mean value of each parameter at that age.
2. **Varying parameters at each age:** We then created an additional 728 virtual subjects at each age by varying each parameter by &#177;1 SD from the mean, and creating a subject with each possible combination of parameters. Only the six most influential parameters were varied (HR, SV, LVET, Diam, PWV, PVR).
3. **Database of simulated pulse waves:** We created a [database](https://peterhcharlton.github.io/pwdb/pwdb.html) of simulated pulse waves for 4,374 virtual subjects (consisting of 729 at each of the six age groups). The database and accompanying code are publicly available.

### Comparison with _in vivo_ Data

We verified this approach for simulating pulse waves for subjects of different ages by comparing the simulated pulse waves with _in vivo_ pulse waves, as shown below:

{{< figure src="https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420006.jpeg" caption="**A comparison between simulated and in vivo pulse wave (PW) shapes. Each pair of plots shows in vivo PWs on the left, and simulated PWs on the right. PWs are shown for different ages in each plot, offset and normalized. Legends indicate ages. <br> _Source: PH Charlton et al., doi: [10.1152/ajpheart.00218.2019](https://doi.org/10.1152/ajpheart.00218.2019) ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)). Some of the in vivo data were obtained from Fluck et al. (doi: [10.3389/fphys.2014.00049](https://doi.org/10.3389/fphys.2014.00049); [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/))_">}}

**Poll Question:** [How well did the model perform?](https://app.sli.do/event/1zunclmb)

<details>
  <summary>A few thoughts</summary>
  
  1. Captured increase in amplitude of second systolic peaks with age in carotid, aortic root and radial pressure waveforms.
  2. Captured disappearance of second peak of finger PPG waveform with age.
  3. Still, some marked differences between _in vivo_ and simulated waveforms.
</details>

Further details of the verification of this approach are provided in the [accompanying article](https://peterhcharlton.github.io/publication/simulating_pulse_waves/).

## Case Study 1: Changes in Pulse Pressure Amplification with Age

## Case Study 2: Assessing Arterial Stiffness from the Photoplethysmogram



## Further Reading and Resources

See the following:
- [Accompanying article](https://peterhcharlton.github.io/publication/simulating_pulse_waves/)
- [Database](https://peterhcharlton.github.io/pwdb/pwdb.html)
- [User Manual](https://github.com/peterhcharlton/pwdb/wiki)
- [Code for case studies](https://github.com/peterhcharlton/pwdb/wiki/Case-Studies)

## Acknowledgment

None of this would have been possible without [Dr Jordi Alastruey-Arimon](http://haemod.uk/members/ja), who provided the [model](http://haemod.uk/nektar) and supervision, and also the British Heart Foundation, who funded the work.


