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
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.container {
  position: relative;
  width: 100%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0.15;
  transition: 2s ease;
  background-color: rgba(0,0,0,0);
}

.container:hover .overlay {
  opacity: 0.7;
}

.text {
  color: white;
  font-size: 10px;
  position: absolute;
  top: 2%;
  left: 50%;
  -webkit-transform: translate(-2%, -2%);
  -ms-transform: translate(-2%, -2%);
  transform: translate(-2%, -2%);
  text-align: center;
}
.container:hover .text {
  opacity: 0;
  display: none;
}

</style>
</head>
<body>
 
<div class="container">
  <img src="../images/landingpage_back.png" alt="wind magnitude" class="image">
<!-- <div class="text">hover me</div> -->
  <div class="overlay">
    <img src="../images/landingpage_winds.gif" alt="wind vectors" class="image">
  </div>
</div>
</body>
</html>

My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with [Dr. Marianna Linz](https://eps.harvard.edu/people/faculty-groups/linz-group) at Harvard University's Department of Earth and Planetary Sciences. More on my [research](https://lrivoire.github.io/research/).

The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of [Earth gazing](https://lrivoire.github.io/earth_gazing/). I also like talking about science with nonscientists, and my [Illustrated science](https://lrivoire.github.io/illustrated_science/) project (coming soon) aims to make my research more accessible to all.

<html>
  <img src="../images/earth.gif" alt="https://earth.nullschool.net/#2020/09/14/2000Z/wind/isobaric/850hPa/overlay=total_precipitable_water/orthographic=-81.84,15.95,421" class="center">
</html>






