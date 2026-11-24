---
title: BeyondFall
date: '2026-05-01'
featured: true
tags:
- Wearable sensing
- ESP32
- Android
summary: A BPPV-aware wearable fall-detection research prototype with an Android companion.
weight: 2
cover_mark: BF
---

**Researcher & Primary System Developer — BeyondFall · May 2026–present**

I implemented ESP32 firmware, inertial sensing, an RBF-SVM classifier, Firebase synchronization and the Android companion app. Features include stable/unstable/fall states, pre-fall haptic warnings, patient-initiated episode logging and SOS alerts.

The experimental evaluation used 990 balanced samples: 495 filtered records from one subject and 495 synthetic normal samples. Reported accuracy was 90.91%, F1 90.82% and ROC-AUC 0.962. These results are preliminary: there were no physician-confirmed vertigo labels or clinical validation. Prototype detection latency was reported below 50 ms.

Demonstrated at JU Innovation Fair 2026. The BeyondFall manuscript is unpublished and is not currently under review.

[Android repository](https://github.com/XtremeseOISHEE/Beyond-Fall) · [ESP32 firmware](https://github.com/XtremeseOISHEE/Beyond-Fall-Arduino-Code-for-IOT-)
