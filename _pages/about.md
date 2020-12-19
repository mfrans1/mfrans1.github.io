---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}

## Hello! My name is Louis and I am an atmospheric scientist.

<html>
<head>
 <style>
   .imageBox {
  position: relative;
  float: left;
}

.imageBox .hoverImg {
  position: absolute;
  left: 0;
  top: 0;
  transition: 5s ease;
  display: none;
}

.imageBox:hover .hoverImg {
  display: block;
  opacity: 0.5;
}
 </style>
</head>
  
<body>
  
  <div class="imageBox">
  <div class="imageInn">
    <img src="../images/landingpage_back.png" alt="wind magnitude">
  </div>
  <div class="hoverImg">
    <img src="../images/landingpage_winds.gif" alt="wind vectors">
  </div>
</div>
</body>
</html>

My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with [Dr. Marianna Linz](https://eps.harvard.edu/people/faculty-groups/linz-group) at Harvard University's Department of Earth and Planetary Sciences. More on my [research](https://lrivoire.github.io/research/).

The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of [Earth gazing](https://lrivoire.github.io/earth_gazing/). I also like talking about science with nonscientists, and my [Illustrated science](https://lrivoire.github.io/illustrated_science/) project (coming soon) aims to make my research more accessible to all.
