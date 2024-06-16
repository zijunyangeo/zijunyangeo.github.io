---
layout: page
permalink: /publications/
title: publications
description: >
  see <a href='https://scholar.google.com/citations?user=yble580AAAAJ&hl=en'>google scholar</a> for most recent publications<br>
  (* denotes equal contribution)
years: [working paper, 2026 , 2025 ,2024, 2023, 2022, 2021, 2020]
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->
<div class="publications">

<!-- {% bibliography %} -->

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
