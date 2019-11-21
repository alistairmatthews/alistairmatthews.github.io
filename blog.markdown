---
title: Blog no Michi
layout: page
---

<h3>A student's progress in Wanomichi Aikido.</h3>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>

{% for post in site.posts %}
  <h2>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </h2>
  {%- assign date_format = site.minima.date_format | default: "%-d %b %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
  {{ post.excerpt }}
  <a href="{{ post.url }}">Read more of this post...</a>
{% endfor %}
