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

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  font-family: Arial;
  font-size: 12px;
}

.container {
  position: relative;
  max-width: 1400px;
  margin: 0 auto;
}

.container img {vertical-align: middle;}

.container .content {
  position: absolute;
  bottom: 0;
  background: rgb(0, 0, 0); /* Fallback color */
  background: rgba(1, 1, 1, 0.5); /* White background with 0.5 opacity */
  color: #f1f1f1;
  width: 100%;
  padding: 20px;
}
</style>
</head>
<body>

<div class="container">
  <img src="../images/landingpage.gif" alt="landing" style="width:150%;">
  <div class="content">
    <h1>Hello! My name is Louis. I am an atmospheric scientist.</h1>
    <p>My research focuses on tropical convection: how it works, how it organizes into phenomena like hurricanes, how it affects the Earth's climate, and how it might change in the future. I work as a postdoctoral fellow with <a href="https://eps.harvard.edu/people/faculty-groups/linz-group">Dr. Marianna Linz</a> at Harvard University's Department of Earth and Planetary Sciences. More on my <a href="https://lrivoire.github.io/research/">research</a>.

The Earth is a wonder of beauty and complexity and I like to extend the concept of stargazing to that of <a href="https://lrivoire.github.io/earthgazing/">Earthgazing</a>. I also like talking about science with nonscientists, and my <a href="https://lrivoire.github.io/illustrated_science/">Illustrated science</a> project (coming soon) aims to make my research more accessible to all.</p>
  </div>
</div>

</body>
</html>

