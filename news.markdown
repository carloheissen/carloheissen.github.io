---
layout: page
title: News
permalink: /news/
---

{% for post in site.posts %}
  <h3>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </h3>
  <p>{{ post.date | date: "%-d %B %Y" }}</p>
  {{ post.excerpt }}
{% endfor %}