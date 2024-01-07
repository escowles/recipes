---
title: dessert
layout: default
---

<h1>{{ page.title }}</h1>
<p>sweets and the component ingredients (crusts, sauces, etc.)</p>

{% assign posts = site.categories.dessert %}
{%- include table.html -%}
