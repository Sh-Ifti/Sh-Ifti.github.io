---
layout: page
title: Saliency Detection with Knowledge Distillation
description: Distilling a large unsupervised saliency model into small networks for edge devices
img: assets/img/projects/saliency_kd.jpg
importance: 1
category: coursework
---

State-of-the-art unsupervised saliency detection relies on large models that are hard to deploy on edge devices. We used knowledge distillation to transfer the behaviour of **PEEKABOO** (a DINO ViT-S/8-based teacher) into two much smaller students: a custom **mini U-Net (~1.9M parameters)** and **U-KAN (~5M parameters)**, a U-Net with Kolmogorov–Arnold Network blocks.

- **Reproducibility study:** retrained PEEKABOO from its public code and compared it against the published weights on ECSSD, DUTS-TEST and DUT-OMRON.
- **Loss design:** KL-divergence distillation failed because the teacher's logits were strongly negative, and ground-truth-masked distillation failed on multi-object images. A weighted mix of BCE (vs. ground truth) and MSE (vs. teacher) worked best.
- **Results:** the U-KAN student reached max F<sub>β</sub> 0.952 and IoU 0.825 on ECSSD in single mode, close to the teacher (0.953 / 0.791), with about 5M parameters. With multi-mode post-processing it reached 0.966 on ECSSD but stayed behind the teacher on the harder multi-object datasets (0.72 vs. 0.86 on DUTS-TEST).

{% include figure.liquid loading="eager" path="assets/img/projects/saliency_kd.jpg" title="mini U-Net" class="img-fluid rounded z-depth-1" zoomable=true %}

<div class="caption">Our mini U-Net student (~1.9M parameters).</div>

Course project (CSE 465), North South University, 2024 · Tanvir Ahmed Khan, Tasin Tayeba Khan, Moshiur Rahman, Shahariar Ifti · PyTorch, DUTS, ECSSD, DUT-OMRON
