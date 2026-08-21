---
layout: page
title: Photos
permalink: /photos/
description: A collection of photos.
nav: true
nav_order: 3
---

<!-- pages/photos.md -->
<!-- Drop image files into assets/img/photos/ and they will show up here automatically. -->

{% assign photos = site.static_files | where_exp: "file", "file.path contains '/assets/img/photos/'" | sort: "path" %}

<div class="row row-cols-2 row-cols-md-3">
  {% for photo in photos %}
    {% assign clean_path = photo.path | remove_first: '/' %}
    <div class="col mb-4">
      {% include figure.liquid path=clean_path class="img-fluid rounded z-depth-1" %}
    </div>
  {% endfor %}
</div>
