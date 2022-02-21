---
layout: page
title: Sediment transport from river plumes
description: 
img: /assets/img/hawkes_2.png

---
This work encompasses the water and suspended sediment movement in Hawke Bay, Aotearoa New Zealand. 

[comment]: <> (There are a important range of scales involved from the nearshore to individual river plumes to inner shelf dynamics.)

I'm using a combination of remote sensing, observational data and numerical ocean modeling to study river plumes, sediment transport, and inner shelf flows.

<img src="/assets/img/s2_plume.png" alt="ex" width="900"/>

images source: European Space Agency, Sentinel-2

#### **Remote sensing of surface sediment concentration**

This work uses satellite remote sensing to study the surface suspended sediment concentration (SSC) in river plumes, which provides detailed spatial information over a long time record of turbid river plume variability. an average annual flux of 11 million tonnes of suspended sediment is transported into the Bay from four main rivers. Remote sensing imagery from MODIS along with an empirical relation between SSC and remote sensing reflectance, determined from in-situ measurements, are used to create daily estimates of surface sediment concentration in the Bay over the last 20 years. Environmental forcing data is used to create a parameter space of how river plumes from individual rivers respond to varying conditions and influence the spatial scales of initial sediment deposition. Current work in  progress uses the SSC gradient in the plumes to estimate ranges of the effective sediment settling velocity.

Code used for Modis processing can be found [here](https://github.com/tedconroy/modis-remote-sensing), and click here(soon)for a poster on this work presented at the Ocean Sciences 2022 Meeting. 

#### **Numerical modeling of river plumes and bay circulation**
COAWST is used to simulate the 3-d flows of the bay and multiple river systems. Multiple nested refinement grids are used to efficiently represent the spatial scales; from the size of the bay to resolving narrow river mouths. Open boundary forcing is sourced from the excellent and open [Moana Hindcast model](https://www.moanaproject.org/hindcast) and atmospheric forcing is from ERA-5.

COAWST matlab set up codes that I use and information about compilation on the NeSI cluster can be found [here](https://github.com/tedconroy/ocean-model-codes/tree/master/coawst).
