---
layout: archive
title: "JetLag, the Lagrangian jet tracking algorithm"
permalink: /JetLag/
author_profile: true
---

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}


![](../images/logo2.png)

**The JetLag data sets and documentation will be released shortly**<br>
Sign up for the [JetLag mailing list](https://web.lists.fas.harvard.edu/mailman/lists/jetlag.lists.fas.harvard.edu/) to be notified.<br>

---

**What is JetLag?**<br>

JetLag is a jet tracking algorithm developed at Harvard University, in collaboration with [Dr. Jezabel Curbelo](https://web.mat.upc.edu/jezabel.curbelo/) at Universitat Politècnica de Catalunya.<br>
JetLag relies on Lagrangian descriptors of the general circulation, hence the name.

---

**Why JetLag?**<br>

Many jet tracking algorithms have been developed in the past, but significant limitations still exist:

* Most algorithms rely on climate-based parameters to detect jet features (e.g. latitude and wind magnitude thresholds, tropopause height gradient). By design, these algorithms cannot be applied to climate studies, and their output is dependent on subjective parameter choices;

  _JetLag employs a non-parametric method by defining jet features as Lagrangian coherent structures_

* Existing algorithms do not explicitely include information about the temporal behavior of the jet, relying instead on the spatial behavior of jet features as seen in instantaneous or time-averaged meteorological fields;

  _JetLag uses time-integrated variables to account for the spatial <em>and</em> the temporal behavior of the jets_

* The majority of algorithms are designed to detect either the subtropical jet or the polar front jet, but not both at the same time. Those that do also rely on climate-based parameters to make the distinction;

  _Jetlag can identify subtropical and polar front jets using a non-parametric classification algorithm_

---

**How does JetLag work?**<br>

The JetLag algorithm uses a Lagrangian descriptor of the general circulation, the 'M function', which is defined at any location (x,y,z,t) as the length of the Lagrangian parcel trajectory initiated at (x,y,z,t) and integrated over a chosen time interval {t-$\tau$ ; t+$\tau$}. The only parameter used in JetLag is the half width of that time interval, $\tau$, which can be determined objectively based on the scales of interest; typical values range from 1 to 3 days.

The M function highlights Lagrangian coherent structures --organizing features of the atmospheric circulation that correspond to maxima in atmospheric transport and that are almost invariant over the chosen integration interval. JetLag uses these features to locate the axes of the jets, ensuring that jet features are coherent both in space and in time.

Once jet features are detected, they are classified as part of the subtropical or the polar front jet by a non-parametric algorithm that makes use of neighborhood rules to ensure that a) the subtropical jet is located equatorward of the polar front jet, b) the most prominent M function features are prioritized, c) jet segments with the same classification do not significantly overlap along the longitudinal dimension.

---

**What will JetLag provide?**<br>

We're still working on it, but we expect to release an ERA5-based beta product in Fall 2023.

Other products will be released over time, including products for the ERAi reanalysis and for CMIP6 model runs.<br>
Contact us (see below) if you are interested in a product that is not available.<br>

---

**Can I get involved?**<br>

Yes! We'd love to hear your thoughts. You can reach out to us via the mailing list (once you've subscribed, email: jetlag-owner (at) lists (dot) fas (dot) harvard (dot) edu) or directly via my professional email (lrivoire (at) fas (dot) harvard (dot) edu). You can request that JetLag be applied to a model output or reanalysis or your choosing –we want JetLag to be useful to your specific purposes! Subject to computing constraints and demand, of course.
