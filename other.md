---
title: other
layout: default
---

<h1>{{ page.title }}</h1>
<p>grab-bag of things, such as dips, drinks, sauces, soap, menus, etc.</p>

{% assign posts = site.categories.other %}
{%- include table.html -%}
