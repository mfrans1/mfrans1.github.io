---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
  
 
<html>
<head>
  <meta charset="UTF-8">
  <title>Image Hover tutorial</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="hover-animation">
  <img src="../images/landingpage.gif" alt="" class="img-back">
  <img src="http://i.stack.imgur.com/Sjsbh.jpg" alt="" class="img-front">
  </div>
</body>
</html>

body{
  background-color=#fff;
}
.hover-animation{
  position: relative;
  height: 400px;
  width: 400px;
  margin: 10% autop 0;
  color: $fff;
}
.hover-animation img{
  position: absolute;
  left: 0;
  top: 0;
  width: 400px;
  height: 400px;
  transition: opacity 2s ease-in-out;
  opacity: 0.6;
}
.hover-animation img.img-front:hover{
  opacity: 0;
  cursor: pointer;
}

 
 
## Hello! My name is Louis and I am an atmospheric scientist.
![](../images/landingpage.gif)

My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with [Dr. Marianna Linz](https://eps.harvard.edu/people/faculty-groups/linz-group) at Harvard University's Department of Earth and Planetary Sciences. More on my [research](https://lrivoire.github.io/research/).

The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of [Earth gazing](https://lrivoire.github.io/earth_gazing/). I also like talking about science with nonscientists, and my [Illustrated science](https://lrivoire.github.io/illustrated_science/) project (coming soon) aims to make my research more accessible to all.
