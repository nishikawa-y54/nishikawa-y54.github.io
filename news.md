---
layout: page
title: NEWS
permalink: /news/
author_profile: false
---

<ul class="news-list">
  {% assign news_posts = site.posts | where_exp: "post", "post.categories contains 'news'" %}
  {% for post in news_posts %}
    <li class="news-item">
      <span class="news-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      &nbsp;
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
