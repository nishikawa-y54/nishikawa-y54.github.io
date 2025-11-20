---
layout: archive
title: "News"
permalink: /news/
author_profile: true
---

{% include base_path %}

{% for post in site.posts %}
  {% if post.categories contains "news" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
