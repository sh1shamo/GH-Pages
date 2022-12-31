---
layout: page
title: Posts
permalink: /posts/
background: '/img/bg-post.jpg'
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>