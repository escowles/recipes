---
title: tags
layout: default
---
{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
  {% assign tag_name = tag | first %}
  <h1 id="{{ tag_name }}">{{ tag_name }}</h1>
  <ul>
    {% assign sorted_posts = tag.last | sort_natural: "title" %}
    {% for post in sorted_posts %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
