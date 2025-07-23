---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}

This is a collection of personal and volunteer projects that I’ve completed outside of formal research settings. Unlike the work featured in the Research section, these projects were not supervised or funded, nor were they conducted for academic credit. Instead, they reflect my own curiosity and drive to apply and expand my skills in data science through self-directed challenges and hands-on learning. 

## Benzie Conservation District Volunteer Data Science Project
Invasive species pose a serious threat to freshwater ecosystems, yet the state of Michigan currently lacks the infrastructure to effectively assess and manage their spread. As part of the Benzie Conservation District’s long-term initiative to develop an aquatic invasive species (AIS) risk assessment for recreational boating and angling pathways in Benzie, Manistee, Grand Traverse, and Leelanau Counties, this project focused on cleaning and analyzing three years of in-situ boater movement data. The raw dataset, compiled from handwritten records collected at regional boat launches, was standardized using fuzzy matching with cosine similarity to align trip entries with the State of Michigan’s official GIS lake registry, resulting in an 89% successful match rate. A network analysis was then performed to identify high-risk transmission pathways between lakes, with interactive Folium maps used to visualize these relationships and inform spatial risk. The resulting insights contribute to ongoing efforts to model AIS spread and have been incorporated into grant proposals for congressional funding to support boat-washing stations and further research.
<figure style="text-align: center;">
  <div style="position: relative; width: 100%; height: 0; padding-bottom: 60%;">
    <iframe src="../files/connections.html" width="100%" height="600" style="border:none;">
    </iframe>
  </div>
  <figcaption style="margin-top: 10px; font-size: 0.9rem; color: #555;">
    Map illustrating frequent recreational boater and angler pathways (>3 occurances) between regional lakes in Northern Michigan. 
  </figcaption>
</figure>

