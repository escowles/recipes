---
title: sides
layout: default
---

<h1 class="section-header">{{ page.title }}</h1>
<p class="section-subhead">side dishes, breads, and other things to accompany main dishes</p>

{% assign posts = site.categories.sides | where_exp: 'item', "item.status != 'deprecated'" %}
{%- include table.html -%}
