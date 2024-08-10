---
title: dessert
layout: default
---

<h1 class="section-header">{{ page.title }}</h1>
<p class="section-subhead">sweets and the component ingredients (crusts, sauces, etc.)</p>

{% assign posts = site.categories.dessert %}
{%- include table.html -%}
