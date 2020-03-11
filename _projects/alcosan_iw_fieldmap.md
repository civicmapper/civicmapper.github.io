---
layout: project
title: ALCOSAN IW Field Map
time: January 2017 - Ongoing
place: Pittsburgh, Pennsylvania, USA
client: ALCOSAN
client-url: https://www.alcosan.org
client-contact: Fred Fields
header-image: alcosan_iw_fieldmap_02.jpg
thumb-image: alcosan_iw_fieldmap_02_thumb.jpg
tags: wastewater infrastructure, laboratory information managment system, field application, research tool, systems integration, ETL, API
project-url: https://iw-fieldmap.civicmapper.com
---

CivicMapper developed the **IW Field Map** web mapping application on behalf of ALCOSAN's Industrial Waste (IW) department. The application's purposes is to enable IW staff to view and access their own permit, sampling, and inspection data (which is stored in another vendor's database) alongside of 3 Rivers Wet Weather (3RWW)-maintained regional wastewater infrastructure geodata. Previously, this was not possible, as the other vendor's data was non spatial and only accessible through their software.

<img class="img-responsive" src="{{site.baseurl}}/assets/img/proj/alcosan_iw_fieldmap_03.jpg"/>

CivicMapper coordinated with that vendor to make their datasets available, and then built an Extract/Transform/Load (ETL) service to push it to the web application's PostgreSQL/PostGIS database. Then, following the Open API-spec, we built a HTTP ReST API to facilitate access to that data. The map was designed with field staff so that it would provides critical information they need in the field with the fewest clicks. To that end, we undertook development iteratively, and conducted user testing early and often.

The application was built with proven open source technologies--Leaflet, PostgreSQL PostGIS, Bootstrap, Flask--in order to prevent vendor lock-in while providing a robust, enterprise-grade web application.