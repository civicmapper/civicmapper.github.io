---
layout: project
title: SUSTAIN Data Extractor
time: April 2015 - Ongoing
place: Pittsburgh, Pennsylvania, USA
client: 3 Rivers Wet Weather
client-url: https://www.3riverswetweather.org
client-contact: Beth Dutton, Program Manager
header-image: trww_sustainextract_01.jpg
thumb-image: trww_sustainextract_thumb.jpg
tags: green infrastructure, stormwater management, ETL, municipal data support, outreach
project-url: https://3rww.github.io/sustain
code-url: https://github.com/3rww/sustain
---

The SUSTAIN Data Extractor is a built-purpose mapping tool for exploring and downloading 3 Rivers Wet Weather's (3RWW) results from an EPA System Urban Stormwater Treatment and Analysis Integration (SUSTAIN) model run for Allegheny County. SUSTAIN is a planning-level site suitability analysis for green stormwater infrastructure (GSI); the modeling work was conducted by 3RWW and finalized May 15, 2013.

This application was built with a very specific purpose: to help municipalities comply with the Pennsylvania Department of Environmental Protection's (DEP) geographic information systems (GIS) map submission requirements of the Phase I Municipal Consent Orders. With this application, 3RWW was able to supply municipalities with the map data needed to address the DEP requirement, at no cost to them.

<img class="img-responsive" src="{{site.baseurl}}/assets/img/proj/trww_sustainextract_03.jpg"/>

This open-source web mapping tool is based on the WPRDC's original [Property Information Extractor](https://github.com/WPRDC/property-information-extractor) prototype, which was based on [Chris Whong's plutoplus](https://github.com/chriswhong/plutoplus). In adapting those tools for this project, we made some big changes under the hood. To utilize ArcGIS Server map services, this version swaps out the [CARTO JS javascript library](https://carto.com/docs/carto-engine/carto-js/) used by those tools for the [Esri-Leaflet javascript library](https://esri.github.io/esri-leaflet).