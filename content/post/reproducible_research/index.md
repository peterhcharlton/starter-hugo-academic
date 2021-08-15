---
title: Making reproducible research as natural as breathing
subtitle: Making research on respiratory rate estimation reproducible.

# Summary for listings and search engines
summary: A short piece on the progress of the RRest project towards making its research entirely reproducible.

# Link this post with a project
projects: [RRest]

# Date published
date: "2016-05-11T00:00:00Z"

# Date updated
lastmod: "2021-08-15T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: P. Charlton'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- reproducible research
- respiratory rate
- wearables

categories:
- Respiratory rate
---

_Written by Peter Charlton whilst a PhD student at King's College London, working on the Hospital of the Future (HotF) project. The overall aim of the HotF project is to provide early identification of hospital patients who are deteriorating. Peter's work focuses on using wearable sensors to continuously assess patients' health._

One of the key aims of the HotF project is to develop a technique to continuously monitor a patient's "respiratory rate": how often they breathe. Respiratory rate often changes early in the progression of a deterioration, giving advanced warning of a severe event such as a heart attack. However, it is currently measured by hand by counting the number of times a patient breathes in a set period of time. This approach is time-consuming, inaccurate, and only provides intermittent measurements. The alternative approach which I'm working on is to estimate respiratory rate from a small, unobtrusive, wearable sensor.

Wearable sensors are currently routinely used to monitor heart rate and blood oxygenation levels. It turns out that the signals which provide these measurements are subtly influenced by respiration, as demonstrated below. If these subtle changes can be extracted reliably, then we could monitor respiratory rate "for free", without the need for any additional sensors. This may provide all-important information on changes in a patient's health, allowing clinicians to identify deteriorating patients earlier.

{{< figure src="featured.png" caption="The heart rate is clearly visible in this signal since each spike corresponds to a heart beat. The spikes also vary in height with each of the four breaths. These subtle changes can be used to estimate respiratory rate.">}}

So what's all this got to do with reproducible research? Well, over the past few decades over 100 papers have been written describing methods for estimating respiratory rate electronically from signals that are already monitored by wearable sensors. If you read them (it takes a long time) then you find that hundreds of methods have been described. The key questions are: which method is the best, and is it good enough to use in clinical practice? Answering these questions can be a daunting task given how many different methods there are. Very few of the methods are publicly available, so to answer these questions you'd have to implement each of the methods yourself. Even once you have done this, you'd need to try them out on some data. Collecting this data is no easy task. Altogether, reproducing scientist's previous work on this problem is quite difficult.

I'm hoping that this won't be such a problem in the future. We have recently implemented many of the methods, collected a benchmark dataset on which to test the methods, and reported the results. All of this is publicly available. What's more, you can [download it all for free](http://peterhcharlton.github.io/RRest/), from the methods, to the data, to the article describing the results. So in a few clicks you can catch up, reproduce our research, and start making progress yourself, even producing methods like this:

{{< figure src="petercharlton_resp_video_gif_red.gif" caption="**Estimating respiratory rate from the electrocardiogram (ECG) and photoplethysmogram (PPG) signals:** A surrogate respiratory signal can be extracted from each of the ECG and PPG signals, which looks similar to a reference respiratory signal (Resp), shown above.">}}

Well, nearly ... I've written a [tutorial](http://peterhcharlton.github.io/RRest/waveform_analysis.html) on the methods, which is due to be published in a textbook soon. This work can be reproduced exactly. Since then we have extended the range of publicly available resources by adding more methods, and the new benchmark dataset. This most recent work can't be reproduced exactly since we had to make a few changes before making it publicly available. I intend to make future work on this topic fully reproducible so that researchers can build on our work. Who knows, perhaps this will contribute towards earlier identification of deteriorating patients in the future.

## Acknowledgment

Originally published [here](https://kingsimaging.wordpress.com/2016/05/11/making-reproducible-research-as-natural-as-breathing/).