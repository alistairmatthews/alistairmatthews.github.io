---
title: Blog no Michi
layout: page
---

<h3>A student's progress in Wanomichi Aikido.</h3>

{% for post in site.posts %}
  <h2>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </h2>
  {{ post.excerpt }}
  <a href="{{ post.url }}">Read more of this post...</a>
{% endfor %}
