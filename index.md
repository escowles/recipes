---
layout: home
---
{% assign posts = site.posts %}
{%- include table.html -%}
<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
