---
layout: page
title: Kitchen Leak Monitor
description: An STM32 system that detects gas leaks and fire in the kitchen and raises an alarm
img: assets/img/projects/kitchen_leak.jpg
importance: 5
category: code
---

A low-cost embedded alarm for gas leaks and kitchen fires, built on an STM32F103 "Blue Pill" for about BDT 2,050 (≈ US$17) in parts. An MQ-2 sensor read through the ADC detects gas and smoke, and a KY-026 sensor detects open flame. An SSD1306 OLED over I2C shows the status, and a buzzer beeps intermittently for smoke and sounds continuously for fire. Firmware written in C with the STM32 HAL, configured in STM32CubeMX and built in Keil µVision.

{% include figure.liquid loading="eager" path="assets/img/projects/kitchen_leak.jpg" title="Prototype" class="img-fluid rounded z-depth-1" zoomable=true %}

<div class="caption">Breadboard prototype with the STM32, MQ-2 and KY-026 sensors, and OLED display.</div>

[Code on GitHub](https://github.com/Sh-Ifti/kitchen-leak-monitor-stm32) · Course project (CSE 331L), North South University, Summer 2024 · with Moshiur Rahman, Pranjal Saha Arnob and Md. Mahedi Hasan
