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
  opacity: 0.1;
  transition: 3s ease;
  background-color: #008CBA;
}

.container:hover .overlay {
  opacity: 0.9;
}

.text {
  color: white;
  font-size: 15px;
  position: absolute;
  top: 2%;
  left: 2%;
  -webkit-transform: translate(-2%, -2%);
  -ms-transform: translate(-2%, -2%);
  transform: translate(-2%, -2%);
  text-align: center;
}

.text:hover {
    display: none;
}

</style>
</head>
<body>

<div class="container">
  <img src="../images/landingpage_back.png" alt="wind magnitude" class="image">
  <div class="text">hover me!</div>
  <div class="overlay">
    <img src="../images/landingpage_winds.gif" alt="wind vectors" class="image">
  </div>
</div>

</body>
</html>


My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with [Dr. Marianna Linz](https://eps.harvard.edu/people/faculty-groups/linz-group) at Harvard University's Department of Earth and Planetary Sciences. More on my [research](https://lrivoire.github.io/research/).

The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of [Earth gazing](https://lrivoire.github.io/earth_gazing/). I also like talking about science with nonscientists, and my [Illustrated science](https://lrivoire.github.io/illustrated_science/) project (coming soon) aims to make my research more accessible to all.


