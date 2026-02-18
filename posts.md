---
layout: page
title: Posts
---

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%B %-d, %Y" }}</p>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
