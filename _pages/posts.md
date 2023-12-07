---
layout: page
title: Blog
image: 01.jpg
permalink: /blog/
---

{% for post in site.posts %}
  <h2><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
  <p>{{ post.date | "%d/%B/%Y" }}</p> <!-- Formats the date -->
  <p>{{ post.excerpt }}</p>
{% endfor %}