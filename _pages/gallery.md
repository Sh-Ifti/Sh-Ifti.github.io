---
layout: page
title: gallery
permalink: /gallery/
description: Photos from fieldwork, workshops, conferences and life in between.
# Set nav to true once you have added a few photos
nav: false
nav_order: 6
---

{% assign photos = site.data.gallery.photos %}
{% if photos and photos.size > 0 %}

<div class="row">
  {% for photo in photos %}
  {% assign img_path = photo.image | remove_first: "/" %}
  <div class="col-sm-6 col-md-4 mt-3">
    {% include figure.liquid loading="lazy" path=img_path title=photo.caption class="img-fluid rounded z-depth-1" zoomable=true %}
    {% if photo.caption %}<div class="caption">{{ photo.caption }}</div>{% endif %}
  </div>
  {% endfor %}
</div>

{% else %}

Photos coming soon.

{% endif %}
