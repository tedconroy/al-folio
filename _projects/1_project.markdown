---
layout: page
title: Coos Estuary dynamics
img: /assets/img/coos_thumb_1.jpeg
---

<div class="img_row">
    <img class="col one left" src="{{ site.baseurl }}/assets/img/pic1.png" alt="" title="example image"/>
    <img class="col two right" src="{{ site.baseurl }}/assets/img/pic3.jpeg" alt="" title="example image"/>
</div>

I worked with [Dave Sutherland](https://www.oceanice.org) and used the [Finite Volume Coastal Ocean Model](http://fvcom.smast.umassd.edu/fvcom/) (FVCOM) for the Coos Estuary in Oregon. The freshwater input into the Coos estuary, and subsequently the hydrography of the estuary and along estuary baroclinic pressure gradient, is highly seasonal (Sutherland and O'Neil 2016), begging the question of how does the estuarine exchange flow, the tidally averaged water movement, change through out the year? To answer this and other questions about the hydrodynamics and salt distribution of the Coos Estuary, we set up FVCOM using high resolution bathymetry mapped onto a high resolution unstructured grid.

<object data="/assets/pdf/Fig1.pdf" type="application/pdf" width="600px" height="800px">
    <embed src="https://github.com/tedconroy/tedconroy.github.io/tree/master">
    </embed>
</object>
(a) Elevation map of the U.S. Pacific Northwest coastline. The shelf break (200-m contour) is shaded in gray, and the numerical model domain is shown in the black outline. The red star shows the location of the Coos Estuary. The main figure shows the bathymetry of the estuary (m referenced to mean sea level) and numerical model domain of the Coos Estuary. The red labels correspond to distance (km) from the mouth of the estuary along the thalweg. The ob- servational stations are labeled numerically on the map, and the corresponding names of the stations are listed in Table 1. (b) The unstructured numerical model grid at the mouth of the estuary, which is outlined in red in the main figure. (c) Depth of the thalweg (m) up the Coos River, Isthmus Slough, and South Slough. (d) Mean cross-sectional area (m2) of channels in (c). The points represent cross sections where flux calculations are performed.

The Total Exchange Flow method (MacCready 2011) was used to quantify the estuarine exchange flow for an annual model run. This method is advantageous because it incorporates both tidal and subtidal motions by using a salinity coordinate instead of an Eulerian coordinate for calculating the exchange flow through cross sections in the estuary. Using the Total Exchange Flow, we found that the tidal component is the dominant component (compared with the subtidal), and that although the along estuary baroclinic pressure gradient changes quite a bit over the year, the inflowing component of the exchange flow doesn't change very much seasonally, but rather with the spring-neap cycle.

<object data="/assets/pdf/Fig7.pdf" type="application/pdf" width="600px" height="400px">
    <embed src="https://github.com/tedconroy/tedconroy.github.io/tree/master">
    </embed>
</object>
 (a) Coos River discharge (m3 s21) over 2014. (b) Tidally filtered total salt content (1010 psu m3) in the estuary throughout 2014 (black line) and the tidally filtered estuarine water volume (108 m3) in orange. (c) The horizontal salinity gradient (psu km21), calculated from the mouth of the estuary up Marshfield Channel and the Coos River, terminating at the depth-averaged 2-psu isohaline. The gray line shows tidal variability while the black line is tidally filtered. (d) Vertical stratification (Ds) at the mouth of the estuary. The gray line is the top to bottom salinity difference (psu) located at a point in the center of the channel, and the black line is tidally filtered. The TEF stratification at the mouth is shown in orange. Note that the Eulerian TEF stratification closely resembles the black line. (e) Eulerian salt flux decomposition evaluated at the mouth of the estuary, including unsteadiness dS/dt, the barotropic river flux FR, the Eulerian flux FEul, and the tidal flux FT.
 
The inflow corresponds with the tidal volume flux, which is converted to a TEF inflow by a number of dispersive processes. There is a strong seasonal component in vertical stratification, mixing (quantified as the dissipation of salinity variance), and the outflowing component of the exchange flow. The seasonality of the outflowing component is important for residence time and transport, especially in the upper reaches of the estuary where the wet season river flux is much larger than the local exchange flow.

<object data="/assets/pdf/Fig9.pdf" type="application/pdf" width="600px" height="400px">
    <embed src="https://github.com/tedconroy/tedconroy.github.io/tree/master">
    </embed>
</object>
(a) The tidal volume flux Qtide (m3 s21) at the mouth of the estuary over 2014. (b) The TEF fluxes (m3 s21) at the mouth of the estuary over the year 2014. The outflowing flux Q is gold, the inflowing flux Q is gray, the inflowing Eulerian flux QEul is orange, and out in in the inflowing tidal flux QTin is blue. (c)–(f) Snapshots of the along-channel variability are shown, which correspond to the times shown in (b) by vertical lines. (g) The year-long average of the exchange flow terms along the main channel.

This work is [now published in the Journal of Physical Oceanography](https://journals.ametsoc.org/doi/abs/10.1175/JPO-D-19-0108.1) with coauthors Dave Sutherland and [Dave Ralston](https://www2.whoi.edu/staff/dralston/). I put some FVCOM processing codes [here](https://github.com/tedconroy/ocean-model-codes).

**References**----------------------------------

Sutherland, D.A. and O'Neill, M.A., 2016. Hydrographic and dissolved oxygen variability in a seasonal Pacific Northwest estuary. Estuarine, Coastal and Shelf Science, 172, pp.47-59.

MacCready, P., 2011. Calculating estuarine exchange flow using isohaline coordinates. Journal of Physical Oceanography, 41(6), pp.1116-1124.
