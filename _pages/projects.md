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

## Monte Carlo Hurricane Track Model with Markov Chains
<figure style="text-align: center;">
  <video controls autoplay muted loop style="width:100%; max-width: 800px;">
    <source src="../files/output.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <figcaption style="margin-top: 8px; font-style: italic; color: #555;">
    Forecasting all hurricanes from 2005-2010 with the statistical model I developed. 
  </figcaption>
</figure>
This project applied 10,000 years of synthetic hurricane track data developed by the Royal Dutch Meteorological Institute to a statistical model aimed at forecasting hurricane tracks between 2005-2010. 
### Building the Transition Matrix for Hurricane Tracks

This function takes the sythetic hurricane track data and converts it into a **transition matrix**, which describes the probability of a storm moving from one grid cell to another. Essentially acting like a roadmap of probabilities, letting us determine: if we start at a point x, where are we **likely** to go for the next step. The chain connecting each step to the next is the markov chain. Our plan: generate these reliably from the data

#### Discretize the tracks
The latitude and longitude of each storm position are mapped onto a regular grid. For example, with a resolution of 0.25° (chosed because it aligns with the resolution of ERA5, will ease the headache of developing the model further in the future), the continuous positions are snapped to the nearest grid cells. Each position is then labeled by its grid cell ID. 

Then for each storm, we look at the sequence of grid cells it passed through. From this sequence, we record all the "hops" between consecutive cells.  
Example: if a storm path visits cells **A → B → C**, we record two transitions: **A→B** and **B→C**.

#### Count how often transitions occur and convert to probabilities
We count the number of times each transition happens across all storms. For example: from cell **A** to cell **B** happened 10 times and from cell **A** to cell **C** happened 5 times.

Then for each starting cell, we divide by the total number of transitions leaving that cell. This gives us the probability of moving from one cell to another. For instance:
- From **A**, the probability to go to **B** = 10 / (10+5) = 0.67  
- From **A**, the probability to go to **C** = 5 / (10+5) = 0.33

#### Transition matrix
All of these probabilities are stored in a square matrix, where:
- Rows = current cell
- Columns = next cell
- Each row sums to 1 (since it represents all possible next steps)

This matrix is the foundation of a **Markov model** that can simulate realistic storm tracks by probabilistically stepping through the grid.

### Monte Carlo Simulation of Storm Tracks

Now we can generate Markov Chains that represent how a hurricane might move through the grid map (the north atlantic basin), but this doesn't really tell us that much. Its just one realization, or observation. We can't do statistics with this. Monte Carlo, essentially running **many** simulations, lets us then take the average track, find the confidence intervals, and have a more robust model. 

#### Run many simulations (padding tracks to equal length)
We start from the same initial storm location, then simulate storm tracks by stepping through the transition matrix. Each track is slightly different, since the next step is chosen randomly according to the transition probabilities.

- Repeat this process `n_tracks` times (for example, 1000 times).
- Each run produces one possible storm path.

Storms may naturally "end" at different times (some dissipate earlier). To compare them fairly:
- We pad shorter tracks with `(NaN, NaN)` values so that all tracks have the same number of steps.  
- This ensures we can store them in a single array and compute statistics across simulations.

#### Compute ensemble statistics
From this collection of tracks, we can compute summary statistics such as:
- **Mean track**: the average latitude and longitude at each time step across all simulations  
- **Spread**: how variable the simulated tracks are (useful for uncertainty estimates)

#### Monte Carlo idea
By simulating a large number of tracks, we approximate the distribution of possible storm paths implied by the transition matrix. The result is not one forecast, but an **ensemble** that captures both the most likely path and the uncertainty around it. We can then apply this approximated distribution to inform our confidence intervals and any other statistics we want to calculate.

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

