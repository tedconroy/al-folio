---
layout: page
title: Hawke Bay
description: 
img: /assets/img/hawkes_2.png

---
This work encompasses the water and suspended sediment movement in Hawke Bay, Aotearoa New Zealand. 

[comment]: <> (There are a important range of scales involved from the nearshore to individual river plumes to inner shelf dynamics.)

I'm using a combination of remote sensing, observational data and numerical ocean modeling to study river plumes, sediment transport, and inner shelf flows.

<img src="/assets/img/s2_plume.png" alt="ex" width="900"/>

images source: European Space Agency, Sentinel-2

# Remote sensing of surface sediment concentration 

Ocean color data from NASA Modis has been used to ... tbc

Code used for Modis processing can be found [here](https://github.com/tedconroy/modis-remote-sensing), and click here(soon)for a poster on this work presented at the Ocean Sciences 2022 Meeting. 

# Numerical modeling of river plumes and bay circulation
COAWST is used to simulate the 3-d flows of the bay and multiple river systems. Multiple nested refinement grids are used to efficiently represent scales from the size of the bay to resolving narrow river mouths. Boundary forcing is sourced from the excellent and open [Moana Hindcast model](https://www.moanaproject.org/hindcast).

COAWST set up matlab codes and information about compilation on NeSI can be found [here](https://github.com/tedconroy/ocean-model-codes/tree/master/coawst).
