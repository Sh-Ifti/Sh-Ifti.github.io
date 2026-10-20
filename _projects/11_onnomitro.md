---
layout: page
title: OnnoMitro
description: Personalized Bangladeshi meal recommendations from a new 305-recipe dataset
img: assets/img/projects/onnomitro.jpg
importance: 4
category: code
---

**OnnoMitro** ("food friend" in Bangla) is a web application that recommends personalized daily meals from traditional Bangladeshi cuisine. Most meal recommenders are built on Western datasets, which makes their suggestions hard to follow in Bangladesh.

**What we built**

- **A new Bangladeshi meal dataset:** 305 recipes collected by web scraping from three Bangladeshi recipe websites, tagged by meal type and vegetarian status, with per-serving calories, carbohydrate, protein, fat and fiber calculated using the Edamam Nutrition Analysis API
- **A recommender system** that estimates each user's energy needs from their metabolic rate, activity level, BMI and goal, splits them into macronutrient targets, and ranks recipes by a weighted nutrient-distance score
- **A Flask web application** with sign-up, a personal dashboard, daily meal plans, alternative suggestions and calorie tracking

{% include figure.liquid loading="eager" path="assets/img/projects/onnomitro.jpg" title="OnnoMitro app" class="img-fluid rounded z-depth-1" zoomable=true %}

<div class="caption">The OnnoMitro app: dashboard, daily meal plan and nutrition overview.</div>

**Results.** On 50 test users, daily recommendations differed from the target calorie intake by a median of 22 kcal (mean absolute error 85.84 kcal). The largest errors came from the uncommon case of users with normal or high BMI who want to gain weight.

[Code on GitHub](https://github.com/Sh-Ifti/onnomitro-meal-recommender) · Senior Design Project (CSE 499), North South University, 2024 · with Tasin Tayeba Khan and Moshiur Rahman, supervised by Dr. Sifat Momen
