---
layout: page
title: Coos Estuary dynamics
img: /assets/img/coos_2.jpeg
---

**Hydrodynamics of the Coos Estuary, Oregon**

<div class="img_row">
    <img class="col one left" src="{{ site.baseurl }}/assets/img/pic1.png" alt="" title="example image"/>
    <img class="col two right" src="{{ site.baseurl }}/assets/img/pic3.jpeg" alt="" title="example image"/>
</div>

I worked with [Dave Sutherland](https://www.oceanice.org) and used the [Finite Volume Coastal Ocean Model](http://fvcom.smast.umassd.edu/fvcom/) (FVCOM) for the Coos Estuary in Oregon. The freshwater input into the Coos estuary, and subsequently the hydrography of the estuary and along estuary baroclinic pressure gradient, is highly seasonal (Sutherland and O'Neil 2016), begging the question of how does the estuarine exchange flow, the tidally averaged water movement, change through out the year? To answer this and other questions about the hydrodynamics and hydrography of the Coos Estuary, we set up FVCOM using high resolution bathymetry mapped onto a high resolution unstructured grid, and ran the model on the University of Oregons supercomputer [Talapas](https://hpcf.uoregon.edu/content/talapas).

<img src="/assets/img/bathy.tif" alt="bathymetry" width="800"/>
*Bathymetry of the estuary (m), showing in-situ observation locations (black), freshwater inputs in the model (blue), and distances from the mouth in km (red).*

The video below is surface salinity (psu) during one of the largest discharge events of 2014 (total freshwater influx was around 800 cubic meters per second), over the course of roughly a week.

<video width="960" height="720" controls>
  <source src="sss.mov" type="video/mp4">
</video>

The Total Exchange Flow method (MacCready 2011) was used to quantify the estuarine exchange flow for an annual model run. This method is advantageous because it incorporates both tidal and subtidal motions by using a salinity coordinate instead of an Eulerian coordinate for calculating the exchange flow through cross sections in the estuary. Using the Total Exchange Flow, we found that the tidal component is the dominant component (compared with the subtidal), and that although the along estuary baroclinic pressure gradient changes quite a bit over the year, the exchange flow doesn't change very much seasonally, but rather with the spring-neap cycle.

This work is now published in the Journal of Physical Oceanography with coauthors Dave Sutherland and [Dave Ralston](https://www2.whoi.edu/staff/dralston/).

**References**----------------------------------

Sutherland, D.A. and O'Neill, M.A., 2016. Hydrographic and dissolved oxygen variability in a seasonal Pacific Northwest estuary. Estuarine, Coastal and Shelf Science, 172, pp.47-59.

MacCready, P., 2011. Calculating estuarine exchange flow using isohaline coordinates. Journal of Physical Oceanography, 41(6), pp.1116-1124.
