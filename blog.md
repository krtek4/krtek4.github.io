---
layout: default
title: Blog
permalink: /blog/
---
{% for post in site.posts %}
  {% assign content = post.excerpt %}
  {% include post.html %}
  _[Read more...]({{ post.url }})_
{% endfor %}
