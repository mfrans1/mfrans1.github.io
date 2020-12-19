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
 
 
.parent {
  position: relative;
  top: 0;
  left: 0;
}
.image1 {
  position: relative;
  top: 0;
  left: 0;
  border: 1px red solid;
}
.image2 {
  position: absolute;
  top: 30px;
  left: 30px;
  border: 1px green solid;
}

<div class="parent">
  <img class="image1" src="../images/landingpage.gif" />
  <img class="image2" src="https://placehold.it/100" />
</div>
 
 
## Hello! My name is Louis and I am an atmospheric scientist.
![](../images/landingpage.gif)

My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with [Dr. Marianna Linz](https://eps.harvard.edu/people/faculty-groups/linz-group) at Harvard University's Department of Earth and Planetary Sciences. More on my [research](https://lrivoire.github.io/research/).

The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of [Earth gazing](https://lrivoire.github.io/earth_gazing/). I also like talking about science with nonscientists, and my [Illustrated science](https://lrivoire.github.io/illustrated_science/) project (coming soon) aims to make my research more accessible to all.
