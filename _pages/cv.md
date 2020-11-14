---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D in Atmospheric Science, Colorado State University, 2020
* M.S. in Ocean, Atmosphere, and Climate Studies, Pierre and Marie Curie University, 2015
* B.S. in Earth Science, Ecole Normale Supérieure, 2013

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
