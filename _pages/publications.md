---
layout: page
permalink: /publications/
title: publications
description: publications by category, in reversed chronological order.
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<h2>Journal Papers</h2>
<div class="publications">
{% bibliography -f papers_journal --group_by none %}
</div>

<h2>International Conference Papers</h2>
<div class="publications">
{% bibliography -f papers_intl_conf --group_by none %}
</div>

<h2>Domestic Conference Papers</h2>
<div class="publications">
{% bibliography -f papers_domestic_conf --group_by none %}
</div>
