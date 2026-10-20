---
layout: page
title: Spondon
description: A US$46 multi-sensor wearable for stress detection (ACM COMPASS 2026)
img: assets/img/projects/spondon.jpg
importance: 1
category: research
---

**Spondon** is a low-cost wearable that detects acute stress from physiological signals, designed for resource-constrained settings where commercial devices (US$300–1,700) are out of reach. It is built from locally available components for about **US$46**.

**Device.** An ESP32 microcontroller with a MAX30102 PPG sensor (heart rate and HRV), a GSR sensor (skin conductance), a GY-906 infrared temperature sensor and an ADXL335 accelerometer, on a custom PCB. Data streams over Wi-Fi to a custom Android app.

**Study.** 15 participants completed a 5-minute baseline, a 5-minute Stroop task and a 5-minute recovery period (NSU IRB-approved).

**Findings.**

- Raw signals generalize poorly to new people (47.9% accuracy), because resting physiology varies widely between individuals.
- Expressing each signal as a change from the person's own baseline raises leave-one-subject-out accuracy to **75.0%** for binary stress detection with a Random Forest.
- Three-class classification (baseline, stress, recovery) reaches 58.4%, against a 33.3% chance level.
- Skin conductance rose significantly during the task (p < 0.001) and was the strongest predictor.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/spondon_gsr.jpg" title="Skin conductance change from baseline" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/spondon_models.jpg" title="LOSO accuracy by model" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>
<div class="caption">
  Left: skin conductance relative to each participant's baseline, rising during the Stroop task (shaded). Right: leave-one-subject-out accuracy by model.
</div>

**Links:** [Paper (ACM Digital Library)](https://doi.org/10.1145/3811242.3819996) · [Analysis code](https://github.com/Sh-Ifti/spondon-stress-wearable)

_Shahariar Ifti, Rahat Jahangir Rony, Shuvashish Chakraborty, Asif Mahbub, Nova Ahmed. ACM COMPASS 2026, short paper._
