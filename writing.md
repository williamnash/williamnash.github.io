---
layout: page
title: Writing
permalink: /writing/
---

<ul class="rows">
  {% for post in site.posts %}
  <li class="row"><span class="when">{{ post.date | date: "%Y" }}</span><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
