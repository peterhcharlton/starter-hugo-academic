---
title: Introduction to modelling arterial pulse waves
summary: An introduction to modelling arterial pulse waves
authors: [admin]
tags: [vascular ageing, pulse waves, arterial stiffness, blood pressure, photoplethysmography]
categories: []
date: "2017-01-01T00:00:00Z"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: white
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
---

## An introduction to modelling arterial pulse waves

Peter Charlton, University of Cambridge, UK 

[peterhcharlton.github.io](https://peterhcharlton.github.io/talk/introduction-to-modelling-arterial-pulse-waves/)

_**To do:** Please go to this website, find this talk under 'Talks', and see the accompanying resources._

---

## I find simulated pulse waves useful for:

1. Understanding physiological mechanisms
2. Designing algorithms
3. Investigating algorithm performance

---

## Accompanying resources

- [The slides](/slides/intro_to_pulse_wave_modelling_slides/): click to expand images
- [The event poll](https://app.sli.do/event/1zunclmb)
- [Accompanying paper](/publication/simulating_pulse_waves/) (from which much content in this presentation is reproduced under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/))

---

# Part 1

## An Introduction to Pulse Wave Modelling using a 1D Model

---

## The Model

[![A 1D Model](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420001.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420001.jpeg)

---

## Simulated Pulse Waves

[![Example simulated pulse waves](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420005.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420005.jpeg)

---

## Model Limitations

**Poll Question:** [What are the limitations of the model?](https://app.sli.do/event/1zunclmb)

---

## Possible Limitations

A few thoughts:

1. Periodic inflow, as opposed to normal heart rate variability
2. Specified arterial properties, which may not be representative of a particular individual
3. Not able to model venous flow

---

## Input Parameters

- HR: heart rate
- SV: stroke volume
- LVET: left ventricular ejection time
- PFT: time of peak aortic flow
- RFV: reverse flow volume
- Diam: the diameters of the largest arteries
- PWV: pulse wave velocities
- MAP: mean blood pressure
- PVC: peripheral vascular compliance

---

## Changing Inputs

Which parameters would be most interesting to change, and why?

Which are most relevant to vascular ageing?

---

## Changing Inputs (2)

[![A 1D Model](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420003.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420003.jpeg)

---

## Changing Inputs (3)

[![A 1D Model](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420002.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420002.jpeg)

---

## Virtual Subjects

We created:
1. Baseline virtual subject at each age
2. Virtual subjects at each age with varying cardiovascular properties
3. A publicly available [database](https://peterhcharlton.github.io/pwdb/pwdb.html) of simulated pulse waves for 4,374 virtual subjects

---

## Comparison with _in vivo_ Data

**Poll Question:** [How well did the model perform?](https://app.sli.do/event/1zunclmb)

[![A 1D Model](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420006.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420006.jpeg)

---

### Thoughts on Performance

- Increase in amplitude of second systolic peaks with age
- Disappearance of second peak of finger PPG with age
- Nonetheless, some marked differences between _in vivo_ and simulated waveforms.

For further details of the verification see the [accompanying article](https://peterhcharlton.github.io/publication/simulating_pulse_waves/).


---

# Part 2

## Case Study: Assessing Arterial Stiffness from the Photoplethysmogram

---

### Digital Wearable Device

[![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/dc/Max_Health_Band.jpg/640px-Max_Health_Band.jpg)](https://upload.wikimedia.org/wikipedia/commons/thumb/d/dc/Max_Health_Band.jpg/640px-Max_Health_Band.jpg)

---

### The Photoplethysmogram (PPG)

[![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Photoplethysmogram_signal_components.svg/640px-Photoplethysmogram_signal_components.svg.png)](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Photoplethysmogram_signal_components.svg/640px-Photoplethysmogram_signal_components.svg.png)

---

### Changes in PPG Pulse Wave Shape

[![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Classes_of_photoplethysmogram_%28PPG%29_pulse_wave_shape.svg/640px-Classes_of_photoplethysmogram_%28PPG%29_pulse_wave_shape.svg.png)](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Classes_of_photoplethysmogram_%28PPG%29_pulse_wave_shape.svg/640px-Classes_of_photoplethysmogram_%28PPG%29_pulse_wave_shape.svg.png)

---

### Assessing Arterial Stiffness

[![](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420004.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420004.jpeg)

---

### Results

[![](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420009.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420009.jpeg)

---

### Implications

1. Age range
2. Influence of HR and SV.

---

### Questions

1. What would you think of using this technology to assess vascular age?
2. How might it compare to other technologies?
3. How could one assess the relative performance of such technologies?

---

### Next Steps

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

---

### Methods

Investigated the effects of age on:
- Early systolic amplification (P1)
- Late systolic pressure augmentation (P2)

at the aorta.

---

### Results

[![](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420008.jpeg)](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420008.jpeg)

---

### Implications

The database can be used to gain insight into the CV determinants of mechanisms of blood flow.

1. When might this be helpful?
2. How should this approach be used:
   - instead of clinical studies
   - as well as clinical studies, or
   - not at all?

---

### Related Work

See the following for similar work, investigating the accuracy of methods for assessing pulse wave velocity:

Willemet M _et al._, _A database of virtual healthy subjects to assess the accuracy of foot-to-foot pulse wave velocities for estimation of aortic stiffness_, doi: [10.1152/ajpheart.00175.2015](https://doi.org/10.1152/ajpheart.00175.2015)

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

---

### Limitations

- Dependent on model accuracy
- Which in turn, is dependent on input parameters
- Often requires specialist knowledge to perform studies

---

### Benefits 

- Allows pulse waves to be simulated under different conditions
- Control of physiology
- Free of measurement error
- Potentially cheap, and doesn't require participant involvement

---

### Opportunities

- Preliminary pilot work in technology development
- Inform the design of _in vivo_ studies
- Understand the potential shortcomings of existing technologies
- Understand the mechanisms underlying haemodynamic observations

--- 

### Further Resources

See the following:
- [Accompanying article](https://peterhcharlton.github.io/publication/simulating_pulse_waves/)
- [Database](https://peterhcharlton.github.io/pwdb/pwdb.html)
- [User Manual](https://github.com/peterhcharlton/pwdb/wiki)
- [Code for case studies](https://github.com/peterhcharlton/pwdb/wiki/Case-Studies)

---

## Acknowledgment

None of this would have been possible without:
- [Dr Jordi Alastruey-Arimon](http://haemod.uk/members/ja), who provided the [model](http://haemod.uk/nektar) and supervision
- The British Heart Foundation, who funded the work
- COST Action CA18216 "Network for Research in Vascular Ageing" supported by COST (European Cooperation in Science and Technology)

---

## Thank you

[peterhcharlton.github.io](https://peterhcharlton.github.io/talk/introduction-to-modelling-arterial-pulse-waves/)

_**See this website for resources.**_
