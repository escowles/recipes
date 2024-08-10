---
title: favorites
layout: default
---

<h1 class="section-header">{{ page.title }}</h1>
<p class="section-subhead">dishes we've made many times, the rock-solid classics</p>

{% assign posts = site.tags.favorite | sort_natural: 'title' %}
{%- include table.html -%}
