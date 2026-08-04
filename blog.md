---
layout: page
title: Blog
permalink: /blog/
---

<div class="blog-layout">
  <aside class="blog-sidebar">
    <h3>Browse by Topic</h3>
    <ul class="topic-list">
      <li><button type="button" class="topic-btn active" data-topic="all">All Posts <span class="topic-count">{{ site.posts.size }}</span></button></li>
      {% assign topics = site.posts | group_by: "topic" | sort: "name" %}
      {% for topic in topics %}
        <li><button type="button" class="topic-btn" data-topic="{{ topic.name }}">{{ topic.name }} <span class="topic-count">{{ topic.items.size }}</span></button></li>
      {% endfor %}
    </ul>
  </aside>

  <div class="blog-main">
    <ul class="post-list">
    {% for post in site.posts %}
      <li class="post-item" data-topic="{{ post.topic }}">
        <div class="post-meta">
          <span class="post-date">{{ post.date | date: "%B %-d, %Y" }}</span>
          {% if post.topic %}<span class="post-badge">{{ post.topic }}</span>{% endif %}
        </div>
        <a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
    </ul>
  </div>
</div>

<style>
  .blog-layout {
    display: flex;
    gap: 3em;
    align-items: flex-start;
  }
  .blog-sidebar {
    width: 180px;
    flex-shrink: 0;
    position: sticky;
    top: 1.5em;
  }
  .blog-sidebar h3 {
    font-size: 0.95em;
    text-transform: uppercase;
    letter-spacing: 0.03em;
    color: #767676;
    margin: 0 0 0.6em;
  }
  .topic-list {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .topic-btn {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    background: none;
    border: none;
    text-align: left;
    font: inherit;
    font-size: 0.95em;
    color: #2a7ae2;
    cursor: pointer;
    padding: 0.35em 0;
  }
  .topic-btn:hover {
    text-decoration: underline;
  }
  .topic-btn.active {
    font-weight: 700;
    color: #111;
  }
  .topic-count {
    color: #999;
    font-size: 0.85em;
    font-weight: 400;
  }
  .blog-main {
    flex: 1;
    min-width: 0;
  }
  .post-list {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .post-item {
    padding: 0.9em 0;
    border-bottom: 1px solid #eaeaea;
  }
  .post-item.is-hidden {
    display: none;
  }
  .post-meta {
    display: flex;
    align-items: center;
    gap: 0.6em;
    margin-bottom: 0.2em;
  }
  .post-date {
    color: #767676;
    font-size: 0.8em;
  }
  .post-title {
    display: block;
    font-size: 1.15em;
    font-weight: 500;
    line-height: 1.3;
  }
  .post-badge {
    font-size: 0.7em;
    color: #555;
    background: #f0f0f0;
    border-radius: 1em;
    padding: 0.15em 0.7em;
  }
  @media (max-width: 700px) {
    .blog-layout {
      flex-direction: column;
      gap: 1.5em;
    }
    .blog-sidebar {
      width: 100%;
      position: static;
    }
    .topic-list {
      display: flex;
      flex-wrap: wrap;
      gap: 0.3em 1em;
    }
  }
</style>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    var buttons = document.querySelectorAll(".topic-btn");
    var items = document.querySelectorAll(".post-item");
    buttons.forEach(function (btn) {
      btn.addEventListener("click", function () {
        buttons.forEach(function (b) { b.classList.remove("active"); });
        btn.classList.add("active");
        var topic = btn.getAttribute("data-topic");
        items.forEach(function (item) {
          var show = topic === "all" || item.getAttribute("data-topic") === topic;
          item.classList.toggle("is-hidden", !show);
        });
      });
    });
  });
</script>
