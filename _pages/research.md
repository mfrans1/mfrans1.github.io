---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}

---
### Tropical cyclone structure and dynamics
![1](../images/TC2.png)
Tropical cyclones have historically been studied from the surface up, in part because their human and ecosystem impacts unfold at the surface, and in part because of the historical scarcity of upper-air observations above open waters.  With the advent of unmanned aircrafts and limb scanning spaceborne instruments, upper-air observations have become more readily available; for example, GPS radio occultation technology now allows the retrieval of the temperature structure in the upper troposphere and lower stratosphere (UTLS) globally, with ~100 m vertical resolution, ~0.1 K accuracy, and in all weather conditions. These data reveal the presence of a ubiquitous, synoptic-scale layer of [cold air near the tropopause above tropical cyclones](https://lrivoire.github.io/publication/2016-09-24-evolution) (and other convective systems), which I call tropopause layer cooling (TLC). The existence of this signal had been documented as early as the 1940s, but its detailed structure and evolution over the lifetime of tropical cyclones had remained unknown until recently. More importantly, the origins of TLC and its potential impacts on the development of the storm below still remain uncertain. Several mechanisms have been proposed to explain TLC, including diabatic cooling at the top of the cloud canopy, and adiabatic cooling due to ascent and divergence. We now know that [cloud radiative effects are unlikely to explain TLC](https://lrivoire.github.io/publication/2020-06-18-quantifying), and I am conducting ongoing research into the mechanisms that main explain ascent and divergence near the tropopause. As to the potential impacts of TLC on the storm below, they include increased potential intensity, turbulence in the outflow layer, heightened clouds, and possible effects on subsequent convection (after the storm has passed). A hierarchical approach with idealized simulations will be necessary to disentangle these effects.

---

### Tropical cyclone risk in future climates
![ ](../images/TC.png)
As the globally averaged surface temperature increases, regional change also occurs. On meso- to synoptic scales, projected changes in atmospheric variables yield changes in both tropical cyclogenesis and in the so-called steering flow that conditions tropical cyclone tracks. Climate simulations lend themselves well to analyzing changes in the steering flow--however, doing so has thus far involved combining complex vortex tracking algorithms, downscaling techniques, and compositing techniques. While these tools have been useful in making projections, their reliance on empirical, arbitrary, or even model-dependent parameters makes them subject to hidden sensitivities, limited reproducibility, and limited applicability. In addition to these shortcomings, climate simulations are not designed to capture the processes at play in tropical cyclogenesis, making risk projections more uncertain. Thus, questions about future tropical cyclone risk remain undoubtedly open, calling for an approach focused on isolating the mechanisms that explain the projected changes. I am currently working on this with collaborators at Purdue and NOAA, using a combination of synthetic tropical cyclone tracks, climate simulations, the historical record of tropical cyclone tracks, and principal component analysis. [Initial results](https://ams.confex.com/ams/34HURR/meetingapp.cgi/Paper/386675) were presented at the AMS 34th Conference on Hurricanes and Tropical Meteorology (May 2021).

---

### Sensitivity of tropical convection to its environment
![ ](../images/convection.png)
Generally speaking, clouds interact with processes on a vast range of scales, from phase changes and interactions with aerosols on microscales to interactions with planetary-scale waves. Cloud systems also interact with each other, both via the circulations they generate and via the atmospheric perturbations they leave behind as they move or dissipate. I am especially interested in the way cloud systems may interact with each other via the tropopause layer cooling (TLC) they generate. General motivation for this work comes from observations of TLC on scales one order of magnitude larger than that of the convective system below, suggesting that cloud systems may interact with each other even at great distances. My research uses a combination of satellite data, idealized simulations with cloud resolving models, and simple theoretical tools such as parcel theory. While this research focuses on meteorological time scales, the results may inform the role of tropical convection on climate time scales.

---

### Atmospheric transport
![ ](../images/transport.png)
The atmosphere mixes and transports a variety of gases and particulates. The distribution of these substances has a significant impact on air quality, on atmospheric chemistry and transport, and on the climate system at large. My research in this area focuses on the transport of ozone between two atmospheric reservoirs with drastically different properties: the troposphere (well mixed, relatively moist, and poor in ozone) and the stratosphere (stratified, very dry, and very rich in ozone). When air parcels that 'originate' in the stratosphere travel downward past the tropopause and into the troposphere (sometimes all the way down to the surface), they bring large amounts of ozone to areas that normally exhibit low concentrations of it. This can trigger air quality issues that affect human and ecosystem health, and that are a regulatory concern. The magnitude of the (downward) cross-tropopause transport of ozone and the processes that lead to it have been the subject of studies since the early 1990s, and remain somewhat difficult to quantify due to satellite coverage and resolution limitations, as well as model resolution limitations. I am currently working with collaborators at Harvard University and at Universitat Politècnica de Catalunya to develop a new jet tracking algorithm that will be the first stepping stone toward taking a new look at this issue. [Initial results](https://meetingorganizer.copernicus.org/EGU22/EGU22-8959.html) will be presented at the 2022 EGU General Assembly.

---

### Stratospheric ozone and circulation
![ ](../images/stratosphere.png)
Stratospheric ozone plays a central role in protecting life on Earth from harmful ultraviolet (UV) radiation from the Sun. Starting in the 1930s, emissions of synthetic compounds such as chlorofluorocarbons (CFCs) have depleted ozone concentrations in the stratosphere, which led to the appearance of the so-called *ozone hole*. The 1987 Montreal Protocol banned the production of CFCs, and their stratospheric concentrations have ever since been decreasing. Over time, this decrease is expected allow stratospheric ozone concentrations to return to their previous levels. However, whether ozone concentrations have already started to recover or not remains a somewhat open question; while the size of the ozone hole has generally decreased since ~2000, large recent variability prevents scienstists from reaching conclusions with a large degree of statistical confidence. At the center of this problem lies the difficult task of establishing a framework to disentangle possible trends in ozone from a multitude of long-term oscillations in the climate system and their complex interactions with changes in the circulation and in the chemical composition of the stratosphere. In addition to this challenge, one must account for the limitations of current observing systems when analyzing long-term trends. I am working with collaborators at Caltech's Jet Propulsion Laboratory and at Princeton's Geophysical Fluid Dynamics Laboratory to provide answers to the question of the statistical significance of the expected ozone recovery. [Initial results](https://ams.confex.com/ams/102ANNUAL/meetingapp.cgi/Paper/398300) were presented at the 21st Conference on Middle Atmosphere of the American Meteorological Society.





