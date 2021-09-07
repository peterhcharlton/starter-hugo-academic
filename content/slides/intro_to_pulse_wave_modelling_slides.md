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

- [The slides](/slides/intro_to_pulse_wave_modelling_slides/)
- [The event poll](https://app.sli.do/event/1zunclmb)
- [Accompanying paper](/publication/simulating_pulse_waves/), from which much content in this presentation is reproduced under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

## The Model

![A 1D Model](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420001.jpeg)

---

## Simulated Pulse Waves

![Example simulated pulse waves](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420005.jpeg)

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

## Model Input Parameters

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

## Changing Model Input Parameters

**Question:** Which parameters would be most interesting to change, and why?

---

## Changing Model Input Parameters (2)

![A 1D Model](https://journals.physiology.org/cms/10.1152/ajpheart.00218.2019/asset/images/large/zh40101929420003.jpeg)

---

# Questions?

[Ask](https://github.com/wowchemy/wowchemy-hugo-modules/discussions)

[Documentation](https://wowchemy.com/docs/managing-content/#create-slides)