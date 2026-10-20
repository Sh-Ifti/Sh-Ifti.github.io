---
layout: page
title: Airbnb Price Prediction
description: Comparing six regression models across ten European cities
img: assets/img/projects/airbnb.jpg
importance: 3
category: code
---

Which model best predicts Airbnb listing prices? This project compares six regression models on listings from ten of Europe's most visited cities. Random Forest performs best, with a test R² of 0.854 against 0.656 for the linear regression baseline.

{% include figure.liquid loading="eager" path="assets/img/projects/airbnb.jpg" title="Predicted vs. actual price" class="img-fluid rounded z-depth-1" zoomable=true %}

<div class="caption">Predicted vs. actual log price on the test set for each model.</div>

[Code on GitHub](https://github.com/Sh-Ifti/airbnb-price-prediction-europe) · Machine Learning course project (CSE 445), North South University, 2024
