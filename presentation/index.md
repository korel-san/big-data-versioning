name: introduce
layout: true
class: center, middle, inverse
---
# Time-based data versioning 
# build with github, mongo and nodejs

.footnote[
  [georgii.rychko@valor-software.com](georgii.rychko@valor-software.com)

  [alexandra.kalinina@valor-software.com](alexandra.kalinina@valor-software.com)
]

???

---

name: data-providers
template: inverse
## Data providers
&nbsp;
#### world-development-indicators
#### unicef

---

name: datasets-differences
template: inverse
## Appreciable differences between
&nbsp;
#### file extensions: xls, csv, json, xml, ...
#### file names: `Cause of death 2015_218f339.xlsx`, `WEOApr2015all.xls`
#### file structures: tabs, columns, extra information ...
#### dimensionalities: `year x country x age x death`, `quarter x region x gini` 
#### units of measurement: `items, thousands, millions`
#### interpretations (specific terms): `MDG region`, `IncSharU`, `IncDefn`

---

name: statistic-issues
template: inverse
## How we could aggregate, analyze and visualize them?
#### visualization library or tool, which could work with large amount of data on frontend
#### creation new standard/specification of the unified data format and query language to it
#### build data server for import/storing/querying all information needed for visualization   

---

name: gapminder-world
template: inverse
## Visualization library (d3js - Vizabi tool)
![](images/GWM2010.png)

???
Show tools page?
---

name: standards
template: inverse
## DDF is a data model for collaborative harmonization 
## of multidimensional statistics.
&nbsp;
![](images/standards.jpg)

???
* **Data model.** DDF is a data model, meaning it describes a way to organize data and to define how pieces of data relate to each other.
* **Harmonization.** DDF can be used for data harmonization, meaning it can combine data from different sources into integrated, consistent and unambiguous data sets. DDF supports a practical workflow that results in an easy to maintain and ever growing collection of comparable data.
* **Collaborative.** DDF is the common data model in open numbers. Open numbers is an initiative to crowdsource and harmonize world-data.
* **Multidimensional statistics.** DDF is designed to store statistics with multiple dimensions. For example population per country, per year, per gender, per age group.

To use DDF effectively, it comes with data formats and a query language. 

---

name: ddf-terms
template: inverse
## DDF terms
#### Datasets
#### Entities (Countries, Quarters, Years, Capitals, Regions)
#### Concepts (Measures, Entity Sets, Entity Domains, Time)
#### Datapoints (Measure, Dimensions, Value)

---

name: ddf-example
template: inverse
## DDF terms
![](images/ddf.png)

???
ddf-light?

---

name: waffle-server
template: inverse
## Waffle Server API per Published DataSet
#### Translated MetaData
#### Availability: Combos of Indicators & Dimensions
#### Stats & Entity properties and hierarchy
#### Geo shapes

---

name: main-goal
template: inverse
## Main goal 
### Provide simple and visualizable tool of 
### time-based data versioning for data scientist 

---

name: main-issue
template: inverse
## Main issue
### Propose a solution to time-based versioning
### for entries and their relations (+)
### and implement storage independable query language (-)

---

name: dependency-graph
template: inverse
## Dependency graph
![](images/dependency_graph.png)

---

name: final-structure
template: inverse
## Final mongodb structure
![](images/final_structure.png)

---

name: infographics
template: inverse
## Infographics
![](images/infographics.png)

---

name: relational-database
template: inverse
## Relational database?

???
(from, to, transactions, originId)

---

template: inverse
# Questions?

???
ddf-light example onair?
 
---
template: inverse
# Thank you

&nbsp;

Contacts:

[georgii.rychko@valor-software.com](georgii.rychko@valor-software.com)

[alexandra.kalinina@valor-software.com](alexandra.kalinina@valor-software.com)
