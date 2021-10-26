---
title: Testing wearables - Part 2
subtitle: Testing wearables for the SAFER Wearables Study

# Summary for listings and search engines
summary: Testing wearable devices for the SAFER Wearables Study - a study investigating the performance and acceptability of wearables for atrial fibrillation screening.

# Link this post with a project
projects: [Safer Wearables]

# Date published
date: "2021-06-15T00:00:00Z"

# Date updated
lastmod: "2021-06-15T00:00:00Z"

# Is this an unpublished draft?
draft: true

# Show this page in the Featured widget?
featured: true

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Devices under test: (from left) a mobile phone, reference ECG chest-patch, electrocardiogram (ECG)-based wristband, and photoplethysmogram (PPG)-based wristband.'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- photoplethysmography
- atrial fibrillation
- electrocardiogram
- SAFER Wearables Study

categories:
- SAFER Wearables Study
- Wearable Devices
- Clinical Studies
---

## Overview

The [SAFER Wearables Study](/project/safer-wearables/) aims to assess the performance and acceptability of wearables for atrial fibrillation screening. It is important that the wearables are able to capture data in everyday life when _unmonitored_ (unsupervised by the researchers - _left to their own devices_).

This post describes initial testing of candidate devices for the study.

## Devices

The devices under test, shown at the top of this page, were:
- **Reference ECG chest-patch**: The [Bittium Faros 180](https://shop.bittium.com/product/36/bittium-faros-180-solution-pack) was used with [long-term electrodes](https://www.ambu.com/cardiology/ecg-electrodes/product/ambu-bluesensor-vlc). It was worn on the sternum, with one electrode placed at the top of the sternum, and the other placed towards the bottom of the sternum (the green, F/LL electrode was not attached). It was set to record a single-lead electrocardiogram (ECG) signal at 125 Hz, with no additional recording (such as accelerometry) or analysis (such as RR-interval derivation). Data were stored on the device for retrospective download via USB.
- **Photoplethysmography-based wristband**: The [Max-Health-Band](https://www.maximintegrated.com/en/products/interface/sensor-interface/MAX-HEALTHBAND.html) was used to record photoplethysmogram (PPG) and accelerometry (accel) signals at the wrist. PPG signals were sampled at 25 Hz (green and ambient), and tri-axis accel signals were also sampled at 25 Hz. The data are initially stored on the device, and transmitted via Bluetooth to a mobile phone for long-term storage (due to limited on-device memory).
- **Electrocardiography-based wristband**: The [Withings Move ECG](https://www.withings.com/uk/en/move-ecg) device was used to acquire 30-second ECG recordings on demand (when the user activated the ECG recording).
- **Mobile phone**: A 'Motorola Moto G8 Power Lite' Android mobile phone was used to store signals from the two wristbands. [Macrodroid](https://www.macrodroid.com/) was used to open and close two apps in turn to download signals from the PPG and ECG wristbands (the '[PulseOn Demo](https://pulseon.com/tech/ohr-tracker)' and '[Withings Health Mate](https://play.google.com/store/apps/details?id=com.withings.wiscale2)' apps respectively). The PPG app was opened twice per hour, for 14 minutes each time, and the ECG app was opened once per hour, for 14 minutes.

## Protocol

A single user attempted to wear the devices for seven days. 
- **Reference ECG chest-patch**: The user changed electrodes if necessary (due to discomfort), but otherwise the device was unattended. The user shaved prior to application, and removed the device for showering.
- **Photoplethysmography-based wristband**: This device was removed and charged each day (typically for 1-2 hours, until it indicated it was fully charged). It was also removed when showering and washing. The device appeared to freeze at one point, so was reset. Otherwise, it was unattended.
- **Electrocardiography-based wristband**: ECG recordings were acquired each day (somewhat sporadically).
- **Mobile phone**: The mobile phone was kept on charge in a room where the user spent several hours each day.

## Outcomes

### User acceptability

The devices were worn for approximately 6.5 days. They were removed early because the ECG chest-patch was sounding a low battery alarm. The user changed one of the chest-patch electrodes twice during the study, and the other one was not changed at all.

### Data acquisition

**Signal samples:** Samples of ECG chest-patch and PPG wristband signals are shown below. These samples were recorded at night, explaining the low heart rate and relatively high signal quality. The PPG signals did not appear to degrade over time. The ECG signals on days 1-3 clearly show P waves, QRS complexes, and T-waves. Several of the PPG signals show two peaks (a systolic and a diastolic peak). This plot demonstrates that it is possible to obtain high quality signals using these devices. However, the ECG signals did appear to be of lower quality from day 5 onwards. Possible explanations for this include: (i) the electrode contact degraded over time (particularly as one of the electrodes was not replaced over the course of the 7 days); and (ii) there was mains interference (such as on Day 6).

{{< figure src="sig_samples.png" caption="**Signal samples over the 7 days of testing:** (left) the reference ECG chest patch; (right) the PPG wristband.">}}

**Inter-beat intervals:** Minute-long samples of ECG chest-patch and PPG wristband signals are shown below, as well as inter-beat intervals derived from the signals. The close agreement between inter-beat intervals derived from the two signals shows that it is possible to obtain reliable inter-beat intervals from these devices.

{{< figure src="IBI_samples.png" caption="**Signals and inter-beat intervals:** obtained from (i) the PPG wristband; (ii) the reference ECG chest patch.">}}

### ECG data quality

Upon further inspection, it became clear that the ECG was of high quality until approximately 4 days (94 hours) into the recording. After then, the ECG was mostly of low quality. The change from high to low quality is shown in the figure below.

{{< figure src="ecg_samples.png" caption="**ECG signals throughout the testing:** Short 2-second samples of ECG signals obtained through the 6.5 days of testing. _Defintion: Hr - hour_">}}

{{< figure src="ecg_change_qual.png" caption="**ECG signals during the second half of testing** Short 2-second samples of ECG signals in the second half of testing. Most samples before 96 hours were of high quality, whereas most after this time point were of low quality. _Defintion: Hr - hour_">}}

## Learning points

We learnt several things from the testing:
1. **Low battery alarm**: The ECG chest-patch sounded a (loud) low battery alarm, waking up the user. I realised that this functionality could have been turned off, and this should be done in the future.
2. **Closing apps**: The process used to close apps was unreliable, and should be refined (perhaps by closing apps one at a time, rather than attempting to close them all using the 'Close All' button.
3. **ECG signal quality**: ECG signal quality may have degraded over the course of the study, so it would be helpful to investigate how often electrodes should be changed (and also whether the presence of mains devices affects ECG signal quality).

## Remaining questions

1. **ECG chest-patch battery life:** Although the device was removed early due to a low battery alarm, it is not clear whether the device could have continued recording for the remaining 0.5 days. When it was connected to a computer the device had approximately 35&#37; battery remaining, indicated that perhaps it could last 7 days. The file size for the ECG signal was 140 MB (leaving over 3GB spare) indicating that the internal storage may be sufficient to store additional signals such as accelerometry, although it's not clear whether turning on the accelerometry would reduce battery life. 
2. **Chest-patch connector**: The chest-patch connector had three electrode connections, but only two were used in this testing. It would be good to find out whether a connector with only two connections is available, which would avoid having a spare connector hanging loosely. 

## Next Steps

Having identified suitable devices for the SAFER Wearables Study, the next steps are:
1. To purchase the necessary devices to start the study
2. To amend the participant-facing documentation to include pictures and detailed instructions on how to use the devices (and submit this for ethical approval).
3. To make the automated data acquisition process (streaming data from wristbands to the mobile phone) as robust as possible.
4. To investigate whether the additional functionality of the ECG chest-patch could be used whilst still having enough battery life.