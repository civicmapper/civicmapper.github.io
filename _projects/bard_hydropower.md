---
layout: project
title: Bard Micro-hydropower Calculator
time: March 2017 - May 2018
place: Pittsburgh, Pennsylvania, USA
client: Bard College and Current Hydro LLC
client-url: 
client-contact: 
header-image: bardhydropower_03.jpg
thumb-image: bardhydropower_thumb.jpg
tags: hydropower, hydrology, web application development, geoprocessing, decision support
project-url: http://bard-hydropower.civicmapper.com
code-url: https://github.com/civicmapper/bard-hydropower
---

The Bard Micro-Hydropower Calculator is a map-based application for estimating the power potential of microhydropower installations. It was built as a demonstration project for [Bard College](http://www.bard.edu/) and [Current Hydro LLC](http://www.currenthydro.com/), and funded by [NYSERDA](https://www.nyserda.ny.gov/).

<img class="img-responsive" src="{{site.baseurl}}/assets/img/proj/bardhydropower_00.jpg"/>

The calculator presents the user with a map-based walkthrough of these steps:

1. **Identify a location for microhydropower, and get information about the terrain**: Use the map and available data layers to identify a spot suitable for a potential microhydropower installation. By diagramming the location of the installation on the map, the calculator will automatically estimate head (elevation change) and delineate the contributing area using available topographic data.
2. **Set calculation parameters**: Set input calculation coefficients and other assumptions used in the calculation (sensible defaults are provided). Optionally, you can also override the head and area estimates derived from map.
3. **See the power potential of a microhydropower installation**. View the analysis results, including total kilowatt hours and estimated revenue generation.

Underlying elevation data driving the calculations is drawn from USGS web services-based geoprocessing tools from [ESRI](https://www.esri.com/en-us/home); where available in New York state, head calculations rely first on high-resolution, LiDAR-derived elevation data services hosted by the [NY State GIS Program Office](http://gis.ny.gov/elevation/DEM-web-services.htm).

<img class="img-responsive" src="{{site.baseurl}}/assets/img/proj/bardhydropower_02.jpg"/>