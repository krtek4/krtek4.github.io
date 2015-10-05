---
layout: default
title: Blog
permalink: /blog/
---
{% for post in site.posts %}
  {% assign preview = true %}
  {% include post.html %}
{% endfor %}
