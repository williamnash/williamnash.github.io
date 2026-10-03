---
layout: page
title: Writing
permalink: /writing/
---

<ul class="post-list">
  {% for post in site.posts %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %Y" }}</time></li>
  {% endfor %}
</ul>
