---
layout: page
title: Regulated Smart Device for Children
description: A parent-controlled smart device design using ARM TrustZone, informed by a parent survey
img: assets/img/projects/child_device.jpg
importance: 3
category: coursework
---

Most parental controls are software that children can work around. This directed research project proposed a **child-specific smart device where parental controls live in hardware**, using the ARM TrustZone secure world of an **STM32L552ZET6** so that screen-time limits and app restrictions cannot be changed from the normal operating system.

- **Parent survey:** we surveyed 46 parents of children under 18 about their background and their children's daily screen time, and analysed it in Python (Mann–Whitney U, Kruskal–Wallis, correlation). Parents' occupational status (r = −0.42) and education (r = −0.35) were negatively associated with children's screen time, while parental age showed almost no relationship.
- **Hardware design:** a 160 × 75 × 9 mm device modelled in Onshape around the TrustZone-enabled microcontroller, with secure boot and protected key storage.
- **Limitations:** the chip and enclosure have not yet been simulated or tested with users.

{% include figure.liquid loading="eager" path="assets/img/projects/child_device.jpg" title="Device design" class="img-fluid rounded z-depth-1" zoomable=true %}

<div class="caption">Technical drawing of the proposed device (Onshape).</div>

Directed research (CSE 498R), North South University, Summer 2024 · Shahariar Ifti, Tasin Tayeba Khan · Supervised by Muhammad Shafayat Oshman
