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

Our planet seen from space, for your perusing and enjoyment.

<html>
<head>
 <style>
 #desc {
   font-size: 15px;
}

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

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="../images/gallery/cira-rammb-slider---meteosat-8---full_disk---geocolor-opacity-100---20201118053000.png">
      <img src="../images/gallery/cira-rammb-slider---meteosat-8---full_disk---geocolor-opacity-100---20201118053000.png" alt="sun glint" width="600" height="400">
    </a>
    <div id="desc">Sun glint over the Indian ocean</div>
  </div>
</div>

<div class="clearfix"></div>

</body>
</html>
