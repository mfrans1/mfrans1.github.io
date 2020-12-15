---
layout: archive
title: ""
permalink: /
redirect_from: 
  - /about/
  - /about.html
author_profile: true
---

{% include base_path %}

{% for post in site.research reversed %} {% include archive-single.html %} {% endfor %}

<html>
.parallax{
    background-image: src="../images/landingpage.gif";
    min-height: 500px; 
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    margin: 0;
}

<title>Bootstrap Default Template</title>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<body>
<h1 id="header">Text</h1>
<div class="parallax"></div>
<div class="col-lg-12 text-box text-center">
</div>
</body>
</html>

