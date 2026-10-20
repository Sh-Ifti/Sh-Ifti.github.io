---
layout: page
title: Sleep Monitoring Wearable
description: An Arduino wrist wearable that estimates sleep and judges the sleep environment
img: assets/img/projects/sleep_wearable.jpg
importance: 1
category: code
---

A low-cost wrist-worn wearable built on an Arduino Uno that records movement (MPU6050), heart rate (PPG pulse sensor) and ambient light through the night and streams the data over Bluetooth. Offline analysis in Python estimates sleep duration from changes in movement and checks whether the room was dark and the heart rate low enough for good sleep.

{% include figure.liquid loading="eager" path="assets/img/projects/sleep_wearable.jpg" title="Overnight signals" class="img-fluid rounded z-depth-1" zoomable=true %}

<div class="caption">Acceleration, light level and heart rate across one recording session.</div>

[Code on GitHub](https://github.com/Sh-Ifti/sleep-monitoring-wearable) · Course project (CSE 323), North South University, 2024
