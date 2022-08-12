---
layout: archive_blog
title: Personal blog
category: blog
permalink: /blog
---

{% for post in site.blog %}
  {% if post.categories contains 'blog' %}
    <div class="post">
        <h3 class="title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="meta">Date: {{ post.date }}</p>
    </div>
  {% endif %}
{% endfor %}