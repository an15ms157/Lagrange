---
layout: archive_photo
title: Personal blog
category: photography
permalink: /photography
---

{% for post in site.post %}
  {% if post.categories contains 'photography' %}
    <div class="post">
        <h3 class="title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="meta">Date: {{ post.date }}</p>
    </div>
  {% endif %}
{% endfor %}

