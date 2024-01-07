---
title: sides
layout: default
---

<h1>{{ page.title }}</h1>
<p>side dishes, breads, and other things to accompany main dishes</p>

{% assign posts = site.categories.sides %}
{%- include table.html -%}
