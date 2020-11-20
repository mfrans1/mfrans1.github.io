---
layout: archive
title: "Earth gazing"
permalink: /earth_gazing/
author_profile: true
---

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}

<html>
<head>
<style>
div.gallery {
  border: 1px solid #ccc;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}

* {
  box-sizing: border-box;
}

.responsive {
  padding: 0 6px;
  float: left;
  width: 24.99999%;
}

@media only screen and (max-width: 700px) {
  .responsive {
    width: 49.99999%;
    margin: 6px 0;
  }
}

@media only screen and (max-width: 500px) {
  .responsive {
    width: 100%;
  }
}

.clearfix:after {
  content: "";
  display: table;
  clear: both;
}
</style>
</head>
<body>

<h2>Responsive Image Gallery</h2>
<h4>Resize the browser window to see the effect.</h4>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="images/gallery/cira-rammb-slider---meteosat-8---full_disk---geocolor-opacity-100---20201118053000.png">
      <img src="images/gallery/cira-rammb-slider---meteosat-8---full_disk---geocolor-opacity-100---20201118053000.png" alt="" width="600" height="400">
    </a>
    <div class="desc">Sun glint over the Indian ocean</div>
  </div>
</div>


<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="">
      <img src="" alt="Forest" width="600" height="400">
    </a>
    <div class="desc">coming soon</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_lights.jpg">
      <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_mountains.jpg">
      <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
    </a>
    <div class="desc">Add a description of the image here</div>
  </div>
</div>

<div class="clearfix"></div>

</body>
</html>
