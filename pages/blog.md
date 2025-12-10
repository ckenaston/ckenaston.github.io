---
layout: page
title: Blog
permalink: /blog
nav_order: 5
---

##Browse by Tag

<ul>
  {% assign tags_list = site.tags | sort %}
  {% for tag in tags_list %}
    <li>
      <a href="/tag/{{ tag[0] | slugify }}/">
        {{ tag[0] }} ({{ tag[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>
