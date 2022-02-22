---
layout: page
title: Sediment transport from river plumes in Hawke Bay
description: 
img: /assets/img/hawkes_2.png

---
This work encompasses the water and suspended sediment movement in Hawke Bay, Aotearoa New Zealand. I'm using a combination of remote sensing, observational data and numerical ocean modeling to study river plumes, sediment transport, and inner shelf flows.

<img src="/assets/img/s2_plume.png" alt="ex" width="900"/>

images source: European Space Agency, Sentinel-2

#### **Remote sensing of surface sediment concentration**

This work uses satellite remote sensing to study the surface suspended sediment concentration (SSC) in river plumes, which provides detailed spatial information over a long time record of turbid river plume variability. an average annual flux of 11 million tonnes of suspended sediment is transported into the Bay from four main rivers. Remote sensing imagery from MODIS along with an empirical relation between SSC and remote sensing reflectance, determined from in-situ measurements, are used to create daily estimates of surface sediment concentration in the Bay over the last 20 years. Environmental forcing data is used to create a parameter space of how river plumes from individual rivers respond to varying conditions and influence the spatial scales of initial sediment deposition. Current work in  progress uses the SSC gradient in the plumes to estimate ranges of the effective sediment settling velocity.

<img src="/assets/img/rs_fig1.png" alt="ex" width="700"/>

<img src="/assets/img/rs_fig2.png" alt="ex" width="700"/>

<img src="/assets/img/rs_fig3.png" alt="ex" width="700"/>

<img src="/assets/img/rs_fig4.png" alt="ex" width="700"/>

Code used for Modis processing can be found [here](https://github.com/tedconroy/modis-remote-sensing), and a poster on this work presented at the Ocean Sciences 2022 Meeting can be found [here](/assets/pdf/tconroy_osm_2022.pdf). 

#### **Numerical modeling of river plumes and bay circulation**
COAWST is used to simulate the 3-d flows and sediment transport of the bay and multiple river systems. Multiple nested refinement grids are used to efficiently represent the spatial scales; from the size of the bay to resolving narrow river mouths. Open boundary forcing is sourced from the excellent and open [Moana Hindcast model](https://www.moanaproject.org/hindcast) and atmospheric forcing is from ERA-5. Below is an example run of sea surface salinity over many tidal cycles, zoomed in on the Wairoa river on the right panel.

<video width="600" controls>
  <source src="/assets/img/coawst_sss.m4v" type="video/mp4">
</video>

COAWST matlab set up codes that I use and information about compilation on the NeSI cluster can be found [here](https://github.com/tedconroy/ocean-model-codes/tree/master/coawst).
