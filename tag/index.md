---
layout: default
title: All Tags
---

<h1>Browse by Tag</h1>

<ul>
  {% assign sorted_tags = site.tags | sort %}
  {% for tag in sorted_tags %}
    <li>
      <a href="/tag/{{ tag[0] | slugify }}/">{{ tag[0] }}</a>
      ({{ tag[1].size }} posts)
    </li>
  {% endfor %}
</ul>
