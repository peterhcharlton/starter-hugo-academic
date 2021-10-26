---
title: 'The Beauty of Biomedical Engineering'
summary: A presentation given in receipt of IPEMs Academic Early Career Award.
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

This transcript accompanies [this talk](/talk/the-beauty-of-biomedical-engineering/).

Some of the transcript content is reproduced from Peter Charlton's [PhD thesis](/publication/cont_resp_monitoring/) under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

## Initial spoken content

On receiving [this prize](/post/ipem_early_career_award/), it might seem appropriate to give a whistle-stop tour of the engineering projects that I've been involved in. My apologies to anyone expecting this, if you're really interested you can read all about our work on [this website](https://peterhcharlton.github.io/). Instead I'm going to share a few thoughts on why Biomedical Engineering is a fantastic field to work in. So, the beauty of Biomedical Engineering.

### The colleagues

Firstly, the colleagues. I've been fortunate to work with great colleagues, who have been an inspiration to me throughout my career.

I was particularly struck by one encounter early in my career. One morning, probably around 10am, a few of us were meeting to discuss a new approach to a problem. An intensive care consultant arrived dressed in scrubs and clutching a cup of coffee. It transpired that he had been on call the previous day, had been up most of the night, and here he was having just handed over, ready to engage in the mathematics of a new signal processing technique, which in the very distant future could potentially help identify the early signs of sepsis. I was inspired by this colleague's dedication, which encourages me to work hard on clinical problems to this day.

Not long later, I was in the same room being introduced to an engineer who had developed a health-monitoring system for jet engines, providing real-time information to ensure the safe passage of air passengers. Now he had turned his attention to a health-monitoring system for people, aiming to spot clinical deteriorations from subtle changes in vital signs. I was inspired by his skill, translating complex analytical techniques across fields, for the benefit of patients.

A year or so later I was at a conference in a mega venue in Brussels, which seemed better suited to debating Members of Parliament than researchers with poster tubes tucked under their arms. One talk described a research study conducted across multiple countries, which had investigated the use of fluid resuscitation to treat children with shock. Whereas this intervention was used everyday in adult intensive care to save lives, the study found it increased mortality in this population - a finding that had apparently baffled the intensive care world. Later that day I attended another session in what felt like a debating chamber, each seat equipped with its own microphone. The chair had asked everyone to speak into their microphones when asking questions. Both the chair and audience quickly became frustrated when one attendee was unable to find the large orange button directly in front of them, with which to turn on their microphone. It was the researcher who'd managed to conduct the baffling study in children across several countries, who finally pointed out that this attendee simply couldn't see their microphone button because their laptop was covering it. I was inspired by her 'smartness', shown by her ability to conduct excellent research, and to solve simple problems which left the rest of us frustrated.

So - the first reason Biomedical Engineering is fantastic - the colleagues.

### The patients

Secondly, the patients. Many, many patients have contributed their time and effort to the research studies I've worked on. Several years ago I helped run a study investigating the use of wearables for monitoring hospital patients. Initially, we expected to equip patients with a miniature gadget, perhaps in the form of a lapel badge, which would transmit their vital signs in real-time to an all-knowing computer, which would quickly identify any problems as they developed. It turned out, in the early 2010s, that such gadgets didn't exist. Instead, we used the existing telemetry devices to monitor patients. These were large devices, about the size of a bag of sugar, that you either had to carry round in your hand, or wear in a shoulder bag slung across your chest. Needless to say, there was a mixed reaction, demonstrated by three patients. 

One patient tolerated the sensor poorly, until it detected that they were having a cardiac arrest and arguably saved their life. Thereafter they tolerated the sensor very well indeed.

One patient was very talkative before their operation, and despite wearing the sensor, died tragically young a few days later.

Finally, one patient, who probably didn't need a sensor, ended up practically dancing around the ward whilst wearing it. I can still see them stood at the nurses station, laughing and joking with the staff on the ward.

So - the second reason Biomedical Engineering is fantastic - the patients.

### The Engineering Problems

Thirdly, the engineering problems. Biomedical engineering problems have all the hallmarks of an exciting engineering project: a problem which we don't understand well, a plethora of innovative solutions, and the potential to save lives. I'll give a very brief example.

---

## Slide: Respiratory Rate

Respiratory rate (RR), the number of breaths taken in a minute, is used in a range of clinical settings for diagnosis and prognosis. [click] Normal RRs lie between 12 and 20 breaths per minute. [click] Elevated RRs have been found to be associated with: [click] COVID-19 diagnosis; [click] admission to intensive care with COVID-19 [click]; and death in hospital with COVID-19. Consequently, it may be helpful to monitor RR to tackle COVID-19.

---

## Slide: Wearables for monitoring Respiratory Rate

Wearables provide a potential opportunity to monitor RR unobtrusively in daily life. [click] Many wearables monitor the pulse at the wrist by measuring an optical signal, the photoplethysmogram (or PPG for short). [click] This signal exhibits a pulse wave for each heart beat, [click] and is also subtly influenced by breathing. Consequently, much research has been conducted on estimating RR from this signal.

---

## Slide: Errors are not normally distributed

Often when taking measurements, such as measuring time or length, one might expect measurement errors to be normally distributed. However, when developing algorithms to estimate RR from wearable sensors, I've been struck that the errors are not necessarily normally distributed. For instance, these plots show the reference RR on the x-axis, and the RR provided by an algorithm on the y-axis. I've repeated the experiment on three different datasets, providing the three plots. Most of the points are clustered around the line of identity, as expected if errors are normally distributed. However, [click] some measurements are very inaccurate, providing erroneously low RRs, which could potentially trigger erroneous clinical responses.

[Click] In this second algorithm, the errors are more normally distributed without the highly erroneous outliers. However, the errors tend to be greater. So we have two algorithms with differing performance characteristics. For this particular problem, it turns out that by combining the two algorithms, one can improve performance, using the upper algorithm to avoid large errors, and the second algorithm to minimise errors.

---

## Closing Slide

We are currently refining the algorithms [click] for use in daily life, and it is my hope that this work will be of great benefit to society.

In case you're interested in this particular problem, you can read more about it and our other work at this website [click]. So - the third reason Biomedical Engineering is fantastic - the challenging problems.

So, to conclude, I think Biomedical Engineering [click] is a fantastic field to work in because of the inspirational colleagues, generous patients, and intriguing engineering challenges. I'd like to thank [click] my funders, and thank IPEM for this prize and the continued support throughout my career.
