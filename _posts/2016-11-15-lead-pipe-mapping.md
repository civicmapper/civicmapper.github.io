---
layout: post
title: Mapping the Lead in Our Water Lines
img: waterlines2.jpg
thumbnail: waterlines_thumb.jpg
author: Emily C. Mercurio & Christian Gass
---

The lead-pipe water crisis in Flint, Michigan in 2015 dramatically raised the awareness of our nation’s municipal water quality and the serious health threats associated with lead pipes, fittings, and solder used in drinking water service lines in American communities.

Elevated lead concentrations in drinking water is not unique to Michigan or here in Pennsylvania, nor is the problem limited to older cities with aging infrastructure: the problem is epidemic across most of the United States. [An Associated Press study from April 2016](http://interactives.ap.org/2016/tainted-at-the-tap/) reported that about 1,400 water systems serving 3.7 million people in 49 U.S. states have exceeded the EPA standard for lead at least once since 2013.

How did this all come to pass? And how does local government tackle such a seemingly massive and complex infrastructure issue?

In this post, we'll look at what organizations have been involved from the federal level on down, what is being asked of local municipalities, and how the local fix starts with a map.

## Directives from the EPA on down
---

In February 2016, the EPA sent [letters to Governors ](https://www.epa.gov/sites/production/files/2016-03/documents/samplelettercommissionersfeb2016.pdf) and [State Commissioners ](https://www.epa.gov/sites/production/files/2016-03/documents/samplelettercommissionersfeb2016.pdf) that called for a plan of action to assess lead levels and ensure that [the Lead and Copper Rule (LCR)](https://www.epa.gov/dwreginfo/lead-and-copper-rule) was being properly implemented. The EPA specifically noted the value of using public websites to disclose lead sampling protocols, lead sampling results and water system inventories of lead service lines.

The EPA stated it will work with states and stakeholders to identify strategies and activities that improve water safety, including technologies that enhance reporting and accountability, and technology solutions that address existing and emerging contaminants. Furthermore, in the letter to State Commissioners, the EPA provided a list of five near-term action items which included the directive to publicly post the locations of lead service lines, including updated inventories or maps of lead service lines and lead plumbing in the system, especially for large systems that serve 50,000 or more people.

### Pennsylvania Responds

In March 2016, [Pennsylvania responded to EPA’s letter ](https://www.epa.gov/sites/production/files/2016-04/documents/pa_response_to_feb_29_letter_508.pdf) and disclosed that **54 of 3,054** water systems in the state did not comply with the Lead and Copper Rule but were in the process of becoming compliant or have initiated corrective action. The letter outlined a general plan for each of the five near-term action items stated in the EPA letter to State Commissioners. It also stated that the commonwealth would work with public water systems to publicly post information that pertains to water sampling and tap locations, but did not imply that the state will help public water systems with mapping of lead service lines.

Development of lead pipe maps, and any other water system distribution maps, will thus be handled by local governments and water authorities. In Pennsylvania, [state code §109.706 defines the requirements for community and noncommunity water system distribution maps.](http://www.pacode.com/secure/data/025/chapter109/chap109toc.html)

### Pittsburgh (and other PA municipalities)

In July 2016, the [Pittsburgh Water and Sewer Authority (PWSA) was ordered by the state Department of Environmental Protection (DEP) to replace lead service lines ](http://www.post-gazette.com/local/city/2016/07/13/PWSA-ordered-to-replace-lead-service-lines-after-elevated-levels-found-in-drinking-water/stories/201607130099) after drinking water testing revealed lead levels above the [EPA maximum standard ](https://www.epa.gov/ground-water-and-drinking-water/basic-information-about-lead-drinking-water#regs) in 17% of homes where lead pipes were suspected or known.

Mr. David Donahoe, the PWSA interim executive director, stated that the **pipeline inventory** will be the biggest challenge because *no centralized currently inventory exists*. Some paper records have been accounted for, and some digital data is available, but a complete, asset-level operational dataset of water service lines does not exist. Pittsburgh is actively replacing lead service lines as they are found during sidewalk repairs and other city maintenance, but this strategy is time-consuming and difficult to quantify or prepare for.

Pittsburgh is one of many areas in the state that has been dealing with elevated lead levels over the past few years. [Lancaster County has identified 17 water systems](http://www.usatoday.com/story/news/nation/2016/03/16/lancaster-county-pa-lead-drinking-water/81576034/) with lead levels above the EPA standard, leading the city of Lancaster to replace 98% of their lead service lines. [Philadelphia has an estimated 60,000 properties with lead service lines of unknown age, but no location maps exist](http://crossroads.newsworks.org/index.php/local/keystone-crossroads/91899-utilities-dont-know-where-lead-pipes-are-and-water-testing-offers-limited-safety-assurances). The problem in Philadelphia is further complicated because the service lines there are private and the Philadelphia Water Department is not responsible for them.

### Successful mapping precedents

The problem shared by most of the affected communities is the lack of an accessible geo-dataset or map that shows where the lead service lines are located. It is impossible to prioritize fixes to a problem of this magnitude with so many gaps in information.

There are great precedents for using geodata and maps to manage this kind of information:

* [Boston Water and Sewer Commission](http://www.bwsc.org/COMMUNITY/lead/leadmaps.asp#TOP_PAGE)
* [District of Columbia Water and Sewer Authority](https://geo.dcwater.com/Lead/)
* [Kalamazoo Department of Public Services](http://www.mlive.com/news/kalamazoo/index.ssf/2016/03/are_your_water_pipes_made_of_l.html)
* [Seattle Public Utilities](http://seattlecitygis.maps.arcgis.com/apps/webappviewer/index.html?id=9a9ad4748a8e41d3bfddd80bc447c3b7).

These maps provide examples of what a web-based lead pipe map can look like and how it can interface with the public.

## An Agile-Data Approach to Lead Water Line Mapping

The urgency of resolving the lead-pipe issue in Pittsburgh and around the country is clear. The question is: where do we start?

First, define what is ultimately needed:

* **a water line inventory, with an emphasis on capturing attributes related to pipe location, materiality (e.g., lead? yes/no) and geometry (e.g., diameter, inverts)**: This inventory forms the basis for addressing the EPA's requirements.

Note that this inventory makes a bunch of other things possible for addressing short- and long-term needs:

* **web map(s) and other tools that support the internal efforts of water authorities**: the water authority can use the data inventory to focus its internal staff and resources. That inventory needs to be built with geospatial technology, which will support the creation of tools that:
  * facilitate data collection
  * identify knowledge gaps and data collection priorities
  * help to prioritize and help manage corrective actions (e.g., pipe replacement)
* **a web map and information site for the public**: There must be a public point of information that relays progress on problem resolution. Maps are great ways to visualize data, but recognizing that not everyone reads maps, the map needs to be a supplement to an easy-to-read informational web page. Transparency will win the day here, and, as we'll explain below, there is no hurdle in making a web map and no excuses for not making one.

Second, make some pragmatic choices about technology and process. To that end, we see three key things that public officials charged with finding the solution to this issue need to push:

**1. Recognize that this is a geospatial data problem first and a civil engineering problem second -- and create the work plan accordingly**

This project demands a design-thinking process applied to a work-planning process: start high-level with data, and iterate down to support detailed engineering requirements.

Focus first on scoping the data picture. Once the data picture begins to become clear, and using tools that leverage geospatial data to answer questions and identify priorities, task civil engineers to do what they are best at: designing solutions for repairing physical infrastructure.

**2. Use available commodity geographic information systems (GIS) products *for the web*, and configure them for the people who are going to use them**

A plethora of web-facing mapping software is available to support this process, is robust and affordable, and can be spun-up quickly. Utilize what is available for cheap--the FOSS4G stack is quite powerful these days--and get someone who knows geospatial technology to tailor it to support the lead pipe mapping data inventory process. An investment in a full-blown, expensive asset management system isn't necessarily required to get started, as any GIS database can transition to that software later on.

**3. Use an agile approach to building the data model and completing the pipe inventory**

With a project of this magnitude, there is a tendency to spec out every last detail of what the data model should look like first: *N* attributes, subtypes, relational tables...? 

*Agile* is a design process often described within the context of software development: *prototype, validate, measure, tweak, repeat*. The result, in software, is often leaner, more focused products that are delivered quickly.

Coincidentally, those are the same characteristics we need of our database and mapping products to tackle the lead pipe problem. Such an approach can be used in building the water line inventory:

* Start with an existing, well-supported data model for water line databases--no need to reinvent the wheel
* Focus on building the dataset out to meet the immediate need using available data sources; emphasize collecting priority records and attributes
* Know that in collecting data, gaps in the data will be revealed--use those to inform continued iteration
* Anticipate consolidating and optimizing the dataset--it's OK to improve how it is structured as more information comes in!
* Plan to evolve the data model as project and organizational needs change (including looking towards a potential transition to asset management software), but don't let that drive the data modeling and collection process at the beginning

*Prototype, validate, measure, tweak, repeat.* As with software, create versioned "releases" of the data. Provide documentation (data model change-logs, data creation assumptions, etc.) that have gone into building each 'release'. Embrace feedback and use it to prioritize the filling of data gaps.

---

In the right hands, the process of collecting the data required to address the lead pipe issue can be performed quite efficiently. More importantly, the process can set the foundation for a long-term data maintenance and asset management strategy.

<br>

## Filling in Data Gaps
---

The use of GIS, geo-enabled databases, and web mapping platforms are keys to success in addressing the lead pipe problem. Obviously, the locations of the lead pipes themselves are key. This begs the question: How do we develop an inventory of lead pipes and service line locations when the data may not exist or has been lost?

This is where the three-part approach above comes into play. A process for building out a dataset filling in data gaps might be comprised for three general steps:

1. Use available data--any data--to identify gaps and next appropriate steps.
2. Work with engineers and experts in the field to:
  * identify tools available for sensor-based lead detection
  * identify places for water sampling campaigns
  * (also: research new techniques for locating lead service lines, building upon what is already known from [testing of previously used technologies](http://www.waterrf.org/PublicReportLibrary/RFR90678_1995_813.pdf)).
3. Use the combination of existing data with sample and sensor data to:
  * drive predictive modeling of missing or incomplete pipe data
  * inform the next round of data collection
  * [plan and visualize pipe-replacement work](https://nextcity.org/features/view/flint-lansing-michigan-replaced-lead-water-pipes)

And repeat. Use the data and web maps to coordinate work internally. Leverage the power of open geospatial tech to communicate results quickly and clearly to the public. Get and build the geo-knowledge needed to get the lead out of our drinking water.

<br>
<hr>

*CivicMapper is a civic tech company that empowers civic organizations to utilize modern mapping technology for the greater good. We think we have some great ideas about tackling the lead pipe problem and would love to help solve it. We are happy to continue the conversation of lead service line mapping and detection, and how we can work together and help your organization develop cost-effective and robust solutions to this challenge:  [info@civicmapper.com](mailto:info@civicmapper.com).*
