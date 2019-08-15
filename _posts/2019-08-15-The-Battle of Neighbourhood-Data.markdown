---
layout: post
title:  "The Battle of Neighbourhood Project"
date:   2019-08-15 20:34:49 +0100
categories: report update
---

## 2.0 Data 
### 2.1 Data Requirements
The dataset or set of data available for this project are:
* Demographics of New York City from U.S. Census of 2000 and the New York Department
of City Planning hosted by [N Y U] [Demographics-of-New-York-Census]
* Demographics of New York City from wikipedia - [Demographics of New York City] [Demographics-of-New-York-City]
* List of Postal Codes of Canada from wikipedia - [Canada List Postal Code] [Canada-List-Postal-Code]
* Boroughs of Nework City from wikipedia - [Boroughs of New York City] [Boroughs-of-New-York-City] 
* Demographics of Toronto Neighbourhoods from wikipedia which is in turn taken from 2006 Canadian Census - [Demographics of Toronto Neighbourhoods] [Demographics-of-Toronto-Neighbourhoods]
* Foursquare API Geolocation data - [Foursquare API] [Foursquare-Developer-API]

The New York City's neighbourhoods dataset for this project is collected from '2000 New York City Neighborhood Names' dataset hosted by NYU’s Spatial Data Repository.
The addresses of the neighbourhoods got from the dataset are used to obtain their equivalent latitude and logitude coordinates of each neighbourhood using geocoder API.

Similarly, Toronto's neighbourhoods data are collected or scraped from the Wikipedia, [Canadian List of Postal Code] [Canada-List-Postal-Code], wrangled, cleaned, then read into a pandas dataframe and structured and formatted like the New York dataset.

The other datasets are to be visualized and drawn an information or insight from them to complement the anlaysis.

The Foursquare API is to be used to acquire data neighborhoods in New York City and Toronto city in terms of common venues and its categories in each neighborhood, and then use these feature to group the neighborhoods or segment(cluster) them.
Foursquare describe a ‘venue’ as a place that one can go to, or check-in.
The Foursquare ‘venue’ is assigned a ‘category’ and each ‘category’ is given a ‘categoryID'



### 2.2 Data Understanding
The datasets are collected based on the data requirements above. The datasets are opened sourced datasets. 
The forms of the two neighbourhoods datasets are in comma separated values with '.csv' extensions. The third dataset is geojson of Toronto City with '.json' extension.
The attributes or characteristics of the data are: 
* identity numbers, 
* longitudes, 
* latitudes, 
* boroughs, 
* neighbourhoods, 
* venue, 
* categories, 
* population, 
* average income, 
* gross domestic product, 
* tips etc.

The latitude is the line running east and west of the earth measured in numeric while
the Longitude is an imaginary line running north and south of Green Wich meridian also measured in numeric.
The borough is a subset of a city. The neighbourhood is the community area name. 

The target value (variable) or label of the data set is the neighbourhood which is the dependent variable. The other variables is like longitudes, latitudes, venues, etc are the independent (predictor) variables.




[Demographics-of-New-York-Census]: https://www1.nyc.gov/site/doh/data/health-tools/neighborhood-statistics-demographics.page

[Demographics-of-New-York-City]:https://en.wikipedia.org/wiki/Demographics_of_New_York_City

[Demographics-of-Toronto-Neighbourhoods]:https://en.wikipedia.org/wiki/Demographics_of_Toronto_Neighbourhoods

[Foursquare-Developer-API]:https://foursquare.com

[Boroughs-of-New-York-City]:https://en.wikipedia.org/wiki/Buroughs_of_New_York_City

[Canada-List-Postal-Code]:https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M
