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
  border-radius: 5px;
}

@keyframes changeopacity {
  from {
    opacity: 0.2;
  }

  to {
    opacity: 0.7;
  }
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  border-radius: 5px;
  background-color: rgba(0,0,0,0);
  animation-duration: 10s;
  animation-name: changeopacity;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}

<!--.container:hover .overlay {
  opacity: 0.7;
}-->

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
<!--.container:hover .text {
  opacity: 0;
}-->
h1 {text-align: center;}



div.textarea {
  text-align: center;
  width: 50%;
  margin-left: auto;
  margin-right: auto;
}

</style>
</head>
<body>
<h1>Hello! My name is Louis.<br>I am an atmospheric scientist.</h1>
  
<div class="container">
  <img src="../images/landingpagebackground.jpg" alt="wind magnitude" class="image">
<!-- <div class="text">hover me</div> -->
  <div class="overlay">
    <img src="../images/landingpagefront.gif" alt="wind vectors" class="image">
  </div>
</div>

<div class="textarea">My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with
<a href="https://eps.harvard.edu/people/faculty-groups/linz-group">Dr. Marianna Linz</a> at Harvard University's Department of Earth and Planetary Sciences. More on my <a href="https://lrivoire.github.io/research/">research</a>.

The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of <a href="https://lrivoire.github.io/earthgazing/">Earth gazing</a>. I also like talking about science with nonscientists, and my <a href="https://lrivoire.github.io/illustrated_science/">Illustrated science</a> project (coming soon) aims to make my research more accessible to all.
</div>

<!--My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with [Dr. Marianna Linz](https://eps.harvard.edu/people/faculty-groups/linz-group) at Harvard University's Department of Earth and Planetary Sciences. More on my [research](https://lrivoire.github.io/research/). The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of [Earth gazing](https://lrivoire.github.io/earthgazing/). I also like talking about science with nonscientists, and my [Illustrated science](https://lrivoire.github.io/illustrated_science/) project (coming soon) aims to make my research more accessible to all.-->

</body>
</html>



