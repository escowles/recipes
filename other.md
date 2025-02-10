---
title: other
layout: default
---

<h1 class="section-header">{{ page.title }}</h1>
<p class="section-subhead">grab-bag of things, such as dips, drinks, sauces, soap, menus, etc.</p>

{% assign posts = site.categories.other | where_exp: 'item', "item.status != 'deprecated'" %}
{%- include table.html -%}
