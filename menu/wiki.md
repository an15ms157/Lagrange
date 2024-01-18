---
layout: default
title: wiki
category: photography
permalink: /wiki
description: "My go-to wiki"

---
<h1>
  {{ page.title }}
</h1>

<h2>Topics</h2>
<ul>
  {% comment %}
    Get all "photo_set" pages and display a list with links to them.
  {% endcomment %}
  {% assign photo_pages = site.pages | where: "layout", "photo_set" %}
  {% for photo_page in photo_pages %}
    <li>
      <a href="{{ photo_page.url | prepend: site.baseurl }}">{{ photo_page.title }}</a>
    </li>
  {% endfor %}
</ul>
