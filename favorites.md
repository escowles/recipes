---
title: favorites
layout: default
---

<h1>{{ page.title }}</h1>
<p>these are the dishes we've made many times, the classics, the rock-solid dishes
we make for company</p>

{% assign posts = site.tags.favorite %}
{%- include table.html -%}
