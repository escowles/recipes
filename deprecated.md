---
title: deprecated
layout: default
---

<h1 class="section-header">{{ page.title }}</h1>
<p class="section-subhead">recipes that have been replaced by other recipes, or otherwise
downgraded to "deprecated" status</p>

{% assign posts = site.posts | where: 'status', 'deprecated' %}
{%- include table.html -%}
