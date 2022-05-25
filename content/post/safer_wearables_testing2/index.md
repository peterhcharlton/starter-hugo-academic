---
title: Testing wearables - Part 2
subtitle: Testing wearables for the SAFER Wearables Study

# Summary for listings and search engines
summary: Testing wearable devices for the SAFER Wearables Study - a study investigating the performance and acceptability of wearables for atrial fibrillation screening.

# Link this post with a project
projects: [SAFER wearables]

# Date published
date: "2021-11-05T00:00:00Z"

# Date updated
lastmod: "2021-11-05T00:00:00Z"

# Is this an unpublished draft?
draft: false

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

Initial testing of candidate devices for the [SAFER Wearables Study](/project/safer-wearables/) was described in [this post](/post/safer_wearables_testing). Two of the key questions remaining after this initial testing were:
1. How often should ECG electrodes be changed to ensure high signal quality?
2. How long does ECG chest-patch battery last?
3. Are chest-patch connectors available with only two electrodes?

This post describes a second round of testing designed to answer these questions.

## Devices

The devices under test were the same as in the first round of testing, with the notable difference of using a different ECG electrode setup, and changing ECG electrodes every 2 days:
- **Reference ECG chest-patch**: The [Bittium Faros 180](https://shop.bittium.com/product/36/bittium-faros-180-solution-pack) was used with [long-term electrodes](https://www.ambu.com/cardiology/ecg-electrodes/product/ambu-bluesensor-vlc). It was worn differently to in the first set of testing. Rather than being worn on the sternum, this time the electrode mounted on the device was attached just below the right clavicle, and one of the cable electrodes was attached just below the ribcage on the left hand side (the green cable was used). This created a lead-II type configuration. It was set to record a single-lead electrocardiogram (ECG) signal at 125 Hz, with no additional recording (such as accelerometry) or analysis (such as RR-interval derivation). The 'battery alarm beep' was turned off, whereas in the first set of testing it had been turned on. Data were stored on the device for retrospective download via USB.
- **Photoplethysmography-based wristband**: The [Max-Health-Band](https://www.maximintegrated.com/en/products/interface/sensor-interface/MAX-HEALTHBAND.html) was used to record photoplethysmogram (PPG) and accelerometry (accel) signals at the wrist. PPG signals were sampled at 25 Hz (green and ambient), and tri-axis accel signals were also sampled at 25 Hz. The data are initially stored on the device, and transmitted via Bluetooth to a mobile phone for long-term storage (due to limited on-device memory).
- **Electrocardiography-based wristband**: The [Withings Move ECG](https://www.withings.com/uk/en/move-ecg) device was used to acquire 30-second ECG recordings on demand (when the user activated the ECG recording).
- **Mobile phone**: A 'Motorola Moto G8 Power Lite' Android mobile phone was used to store signals from the two wristbands. [Macrodroid](https://www.macrodroid.com/) was used to open and close two apps in turn to download signals from the PPG and ECG wristbands (the '[PulseOn Demo](https://pulseon.com/tech/ohr-tracker)' and '[Withings Health Mate](https://play.google.com/store/apps/details?id=com.withings.wiscale2)' apps respectively). The PPG app was opened twice per hour, for 14 minutes each time, and the ECG app was opened once per hour, for 14 minutes. The WiFi was kept turned off (apart from a brief period of it being turned on, on the first day).

## Protocol

A single user attempted to wear the devices for seven days. 
- **Reference ECG chest-patch**: The user changed electrodes every two days, but otherwise the device was unattended. The user shaved prior to application, and removed the device for showering.
- **Photoplethysmography-based wristband**: This device was removed and charged each day (typically for 1-2 hours, until it indicated it was fully charged). It was also removed when showering and washing. Otherwise, it was unattended.
- **Electrocardiography-based wristband**: ECG recordings were acquired on an _ad-hoc_ basis.
- **Mobile phone**: The mobile phone was kept on charge in a room where the user spent several hours most days.

## Outcomes

### User acceptability

The devices were worn for the full 7 days. ECG electrodes were changed every two days as planned.

### ECG Chest-Patch data quality

The ECG chest-patch data appeared to remain high quality throughout the recordings, as shown by the snapshots of ECG signal below, from throughout the 7 days.

{{< figure src="ecg_samples_pt2.png" caption="**ECG signals throughout the testing:** Short 2-second samples of ECG signals obtained through the 7 days of testing. _Defintion: Hr - hour_">}}

### Chest-patch battery

At the end of the 7 days, the ECG chest-patch was disconnected. At this point the blue battery light was flashing, but the low battery alarm didn't sound (as planned, because it was turned off). When the chest-patch was connected to a computer for data download, it said:
- 11% charge remaining
- 85% free memory

### Leads with only two electrodes

Following the testing, we were able to purchase ECG leads with only two electrodes, removing the need for a third electrode. The leads purchased are not long enough for a lead-II configuration, so will be used across the sternum.

## Learning points

We learnt several things from the testing:
1. **ECG signal quality**: The chest-patch ECG data was of high quality through this test, indicating that high quality data can be obtained for 7 days, and suggesting that it might be helpful to change the electrodes every 2 days to help ensure high quality data.
2. **Chest-patch battery**: The chest-patch battery did last for the full 7 days (albeit the low battery light was flashing by the end), indicating that the battery can last for 7 days.
3. **Chest-patch memory**: It appears that there is plenty of spare memory on the chest-patch device after a 7 day recording, so potentially accelerometry data could be acquired simultaneously (if that does not affect battery life too much).

## Remaining questions

1. **Accelerometry**: Is it possible to acquire accelerometry data too, and still have enough battery lifetime for 7 days of data acquisition?

## Next Steps

Having identified suitable devices for the SAFER Wearables Study, the next steps are:
1. To purchase the necessary devices to start the study
2. To amend the participant-facing documentation to include pictures and detailed instructions on how to use the devices (and submit this for ethical approval).
3. To make the automated data acquisition process (streaming data from wristbands to the mobile phone) as robust as possible.
4. To investigate whether the additional functionality of the ECG chest-patch could be used whilst still having enough battery life.