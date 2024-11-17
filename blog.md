---
layout: page
title: Blog
permalink: /blog/
---

# Blog

Welcome to my blog! Below is a list of all my posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>
