---
layout: archive
title: "NEWS"
permalink: /news/
author_profile: false
---

{% include base_path %}

{% for post in site.categories.news %}
  {% include archive-single.html %}
{% endfor %}
