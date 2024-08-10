---
title: main
layout: default
---

<h1 class="section-header">{{ page.title }}</h1>
<p class="section-subhead">main dishes, or the key component of a meal</p>

{% assign posts = site.categories.main %}
{%- include table.html -%}
