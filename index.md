---
layout: home
---
{% assign posts = site.posts | where_exp: 'item', "item.status != 'deprecated'" %}
{%- include table.html -%}
<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
