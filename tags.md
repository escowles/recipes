---
title: tags
layout: default
---
# tags
{% assign sorted_tags = site.tags | sort %}

<ul class="taglist">
{% for tag in sorted_tags %}
  {% assign tag_name = tag | first %}
  {% assign tag_posts = tag | last %}
  <li class="tagnav"><a href="{{"/" | relative_url }}?q={{ tag_name }}">{{ tag_name }}</a> ({{ tag_posts.size }})</li>
{% endfor %}
</ul>
