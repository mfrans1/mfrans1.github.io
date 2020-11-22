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

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="../images/gallery/cira-rammb-slider---goes-16---full_disk---geocolor-opacity-100---20170905104534.png">
      <img src="../images/gallery/cira-rammb-slider---goes-16---full_disk---geocolor-opacity-100---20170905104534.png" alt="irma" width="600" height="400">
    </a>
    <div id="desc">Sunrise over hurricane Irma as it heads for the Caribbean</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201118232031.png">
      <img src="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201118232031.png" alt="vortex_street" width="600" height="400">
    </a>
    <div id="desc">Vortex street south of Isla Guadalupe</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201119013031.png">
      <img src="../images/gallery/cira-rammb-slider---goes-17---full_disk---geocolor-opacity-100---20201119013031.png" alt="" width="600" height="400">
    </a>
    <div id="desc">Waves in clouds near Hawai'i</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="../images/gallery/cira-rammb-slider---goes-16---full_disk---geocolor-opacity-100---20201119200014.png">
      <img src="../images/gallery/cira-rammb-slider---goes-16---full_disk---geocolor-opacity-100---20201119200014.png" alt="" width="600" height="400">
    </a>
    <div id="desc">Swirly clouds in the south Pacific</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="../images/gallery/cira-rammb-slider - -himawari - -full_disk - -geocolor-opacity-100 - -20201121190000-20201121235000.gif">
      <img src="../images/gallery/cira-rammb-slider - -himawari - -full_disk - -geocolor-opacity-100 - -20201121190000-20201121235000.gif" alt="knife cuts" width="600" height="400">
    </a>
    <div id="desc">"Knife cut" waves near Australia</div>
  </div>
</div>

<div class="clearfix"></div>

</body>
</html>
