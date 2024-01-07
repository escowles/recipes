---
title: main
layout: default
---

<h1>{{ page.title }}</h1>
<p>main dishes, or the key component of a meal</p>

{% assign posts = site.categories.main %}
{%- include table.html -%}
