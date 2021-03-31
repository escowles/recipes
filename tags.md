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
  <li class="tagnav"><a href="#{{ tag_name }}">{{ tag_name }}</a> ({{ tag_posts.size }})</li>
{% endfor %}
</ul>

{% for tag in sorted_tags %}
  {% assign tag_name = tag | first %}
  <h2 id="{{ tag_name }}">{{ tag_name }}</h2>
  <ul>
    {% assign sorted_posts = tag.last | sort_natural: "title" %}
    {% for post in sorted_posts %}
      <li class="taglink"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
