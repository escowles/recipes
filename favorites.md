---
title: favorites
layout: default
---

<h1>{{ page.title }}</h1>
<p>dishes we've made many times, the rock-solid classics</p>

{% assign posts = site.tags.favorite | sort_natural: 'title' %}
{%- include table.html -%}
