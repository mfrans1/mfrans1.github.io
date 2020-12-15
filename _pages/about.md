---
layout: archive
title: ""
permalink: /
redirect_from: 
  - /about/
  - /about.html
author_profile: false
---

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}

