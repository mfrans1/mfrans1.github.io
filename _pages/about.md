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
  margin-bottom: 1cm;
  margin-top: 1cm;
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
  animation-duration: 8s;
  animation-name: changeopacity;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}

.overlaytext {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  background-color: rgba(0,0,0,0);
  color: white;
}
.container:hover .overlaytext {
  opacity: 1;
}

<!--.container:hover .overlay {
  opacity: 0.7;
}-->

<!--.text {
  color: white;
  font-size: 10px;
  position: absolute;
  top: 2%;
  left: 50%;
  -webkit-transform: translate(-2%, -2%);
  -ms-transform: translate(-2%, -2%);
  transform: translate(-2%, -2%);
  text-align: center;
}-->
<!--.container:hover .text {
  opacity: 0;
}-->
h1 {text-align: center;}

div.textarea {
  text-align: justify;
  text-justify: inter-word;
  width: 80%;
  margin-left: auto;
  margin-right: auto;
}

.irma { 
  position: absolute; 
  top: 75%; 
  left: 48%;
  opacity: 0;
  color: white;
  text-align: center;
  font-size: 1vi;
} 
.katia { 
  position: absolute; 
  top: 65%; 
  left: 12.5%;
  opacity: 0;
  color: white;
  text-align: center;
  font-size: 1vi;
} 
.jose { 
  position: absolute; 
  top: 93.5%; 
  left: 77.5%;
  opacity: 0;
  color: white;
  text-align: center;
  font-size: 1vi;
} 
.copyright { 
  position: absolute; 
  bottom: -0.4cm; 
  right: 0.1cm;
  opacity: 0;
  color: black;
  text-align: right;
  font-size: 10px;
} 
.joseeyes { 
  position: absolute; 
  top: 80%; 
  left: 79%;
  opacity: 0;
  width: 4%;
} 

.container:hover .irma {
  opacity: .8;
  transition: 0.4s;
  transition-delay: 0.15s;
  transform: translateY(-1cm);
  transition-timing-function: ease;
}
.container:hover .katia {
  opacity: .8;
  transition: 0.4s;
  transform: translateY(-1cm);
  transition-timing-function: ease;
}
.container:hover .jose {
  opacity: .8;
  transition: 0.4s;
  transition-delay: 0.3s;
  transform: translateY(-1cm);
  transition-timing-function: ease;
}
.container:hover .copyright {
  opacity: 1;
  transition: 1s;
  transition-delay: 1s;
  transition-timing-function: ease;
}
.container:hover .joseeyes{
  opacity: 1;
  transition: 0.1s;
  transition-delay: 10s;
  transition-timing-function: ease;
}

</style>
</head>
<body>
  
<h1>Hi! My name is Louis, I am an atmospheric scientist.</h1>
  
<div class="container">
  <img src="../images/landingpagebackground.jpg" alt="wind magnitude" class="image">
<!-- <div class="text">hover me</div> -->
  <div class="overlay">
    <img src="../images/landingpagefront.gif" alt="wind vectors" class="image">
  </div>
  <div class="irma">
    Irma
  </div>
  <div class="katia">
    Katia
  </div>
  <div class="jose">
    Jose
  </div>
  <div class="copyright">
    <a href="https://earth.nullschool.net/#2017/09/08/0200Z/ocean/isobaric/1000hPa/overlay=significant_wave_height/orthographic=-77.92,20.64,1100">earth.nullschool.net</a>
  </div>
</div>

<div class="textarea">I am primarily interested in the role of the upper troposphere and lower stratosphere in the climate. I also work to understand how sampling biases and observational uncertainties affect our understanding of the climate. <br><br> <!--For instance, as the Earth continues to warm, the behavior of the jet streams changes, affecting the transport of stratospheric ozone into the boundary layer, the location of tropical cyclone landfalls, and the intensity of the stratospheric circulation.-->
My work is driven by applications in atmospheric composition, air quality, and hurricane risk.
I work as a Postdoctoral Associate with
<span style="white-space:nowrap"><a href="https://www.teampaccc.mit.edu/">Dr. Arlene Fiore</a></span> at MIT's department of Earth, Atmospheric and Planetary Sciences.<br><br>-->
</div>
</body>
</html>
<!--In all my research projects I strive to develop objective methods that can be applied for the analysis of the atmosphere regardless of the state of the climate. 
</div>
<!--The Earth is a wonder of beauty and complexity, and I like spending time <a href="https://lrivoire.github.io/earthgazing/">Earthgazing</a>. I also like talking about science with nonscientists, and my <a href="https://lrivoire.github.io/illustrated_science/">Illustrated science</a> project (coming soon) aims to make my research more accessible to all.-->
<!--My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with [Dr. Marianna Linz](https://eps.harvard.edu/people/faculty-groups/linz-group) at Harvard University's Department of Earth and Planetary Sciences. More on my [research](https://lrivoire.github.io/research/). The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of [Earth gazing](https://lrivoire.github.io/earthgazing/). I also like talking about science with nonscientists, and my [Illustrated science](https://lrivoire.github.io/illustrated_science/) project (coming soon) aims to make my research more accessible to all.


