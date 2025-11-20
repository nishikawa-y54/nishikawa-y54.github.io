---
layout: page
title: NEWS
permalink: /news/
author_profile: false
---

<ul class="archive__list">
  {%- assign news_posts = site.categories.news | sort: "date" | reverse -%}
  {%- for post in news_posts -%}
    <li class="archive__item">
      <span class="archive__item-date">
        {{ post.date | date: "%Y-%m-%d" }}
      </span>
      &nbsp;
      <a class="archive__item-title" href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </li>
  {%- endfor -%}
</ul>
