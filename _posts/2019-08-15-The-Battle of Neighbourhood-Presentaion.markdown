---
layout: post
title:  "The Battle of Neighbourhood - Presentation"
date:   2019-08-15 20:34:49 +0100
categories: report update
---

## 1.0 Introduction
### 1.1 Problem 
Mujaware Services LLC wants to open (restaurant) business but doesn't know which one of these two neighbourhoods, the Manhattan and the Downtown in the New York City and the Toronto City respectively, is better to open or cite a company or business. 
Hence the problem is
how to determine the right neighbourhood for Mujaware Services LLC to open a (restaurant) business.
### 1.7  Background

Muware Services LLC is service-rendering company that has been in existence for several years. This year, the management of the company is planning of expanding their services to one of the two cities' neighbourhoods of the New York City and the Toronto City. 

The New York City and the Toronto city are both cities in different countries United States and Canada respectively. The two respective neighbourhoods that is of interest here are the Manhattan in the New York City and and the Downtown in Toronto.
## 2.0 Data

### 2.1 Source of Data
The dataset or set of data available for this project are:
* Demographics of New York City from U.S. Census of 2000 and the New York Department
of City Planning hosted by [N Y U] [Demographics-of-New-York-Census]
* Demographics of New York City from wikipedia - [Demographics of New York City] [Demographics-of-New-York-City]
* List of Postal Codes of Canada from wikipedia - [Canada List Postal Code] [Canada-List-Postal-Code]
* Boroughs of Nework City from wikipedia - [Boroughs of New York City] [Boroughs-of-New-York-City] 
* Demographics of Toronto Neighbourhoods from wikipedia which is in turn taken from 2006 Canadian Census - [Demographics of Toronto Neighbourhoods] [Demographics-of-Toronto-Neighbourhoods]
* Foursquare API Geolocation data - [Foursquare API] [Foursquare-Developer-API]

### 2.2 Data Description
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

## 3.0 Research Methodology/Tools

### 3.1 Exploratory Data Analysis
The data sets of the two neighbourhoods, the Downtown and the Manhattan were visualized to gain knowledge of the distribution of variables and the neighbourhoods in the Boroughs, the Downtown and the Manhattan, using folium library to see how the neighbourhoods in this borough are spatially distributed. The resulting data is subjected to initial step of data analysis – the exploratory data analysis (EDA) to gain insight on how correlated or trending the data are.
After the data sets have been subjected to exploratory data analysis using Folium, Seaborn and Matplotlib libraries to see how the variables of the data are distributed, trending and insight gained, the data was then subjected to pre-processing stage.

### 3.2    Inferential Statistical Testing Techniques (Machine Learning)
Here the encoded data during the analysis are fed into the machine learning algorithm - K-mean Clustering - to group or segment the neighbourhoods. At the end, the neighbourhoods that have similar characteristics are grouped together. Thence the similarities and dissimilarities of the Downtown and the Manhattan are observed.

## 4.0 Results
Table 1: First Five of Group of Neighbourhoods and Venues of the Manhattan
![Manhattan Groupby](/images/manhattan-groupby.JPG)

Table 2: First Five of Group of Neighbourhoods and Venues of the Downtown
![Downtown Groupby](/images/downtown-groupby.JPG)

Table 3: The Most Common Venues of the First Five Neighbourhoods of the Downtown
![Downtown Venues](/images/downtown-venues.JPG)

Table 4: The Most Common Venues of the First Five Neighbourhoods of the Manhattan
![Manhattan Venues](/images/manhattan-venues.JPG)

Table 5: First Five Cluster Neighbourhoods of the Downtown
![Downtown Cluster](/images/downtown-cluster.JPG)

Table 6: First Five Cluster Neighbourhoods of the Manhattan
![Manhattan Cluster](/images/manhattan-cluster.JPG)

Figure 1: The Downtown's Map Showing Neighourhood and Venues
![Downtown Venues Map](/images/downtown-venues-map.JPG)

Figure 2: The Manhattan's Map Showing Neighourhood and Venues
![Manhattan Venues Map](/images/manhattan-venues-map.JPG)

Figure 3: The Manhattan's Map Showing Neighourhoods and Venues' Clusters
![Manhattan K Mean](/images/manhattan-kmean.JPG)

Figure 4: The Downtown's Map Showing the Neighbourhoods and Venues' Clusters
![Downtown K Mean](/images/downtown-kmean.JPG)

## 5.0 Discussion
### 5.1 Observations
The two neighbourhoods in the Manhattan of the New York City and the Downtown Toronto of the Toronto City - are similar in having banks, grocery, market, farmers market, waterfall, college, transport station and buildings but dissimilar in other venues listed above and in the table 2.5 shown above in the result section.

These venues that are similar indirectly represent availability of capital made available by bank, raw materials provided by the farmers markets and groceries, water provided by waterfall, labour provided by the colleges and the universities, efficient management provided by the college and the competitors which are in the restaurant businesses in the neighbourhoods, transport facilities provided by the presence of bus or train stations in the neighbourhoods.

### 5.5 Recommendations
Even though there are factors that are not available during the research, the research still recommend that the Manhattan neighbourhoods should be considered in citing a restaurant business if the two boroughs given to be considered are the Manhattan and the Downtown.
## 6.0 Conclusion
In the end, the Manhattan neighbourhoods are better than the Downtown neighbourhoods in citing a restaurant business based on the available data. Why? Though the two neighbourhoods are similar in factor that influence the location of restaurant business yet they are glaringly dissimilar in the population densities and hence the market shares of a potential restaurant business.
Any potential restaurant businesses cite in the Manhattan will have large market share because of the population or population density of the area than if it is to be cited in the Downtown.

[Demographics-of-New-York-Census]: https://www1.nyc.gov/site/doh/data/health-tools/neighborhood-statistics-demographics.page

[Demographics-of-New-York-City]:https://en.wikipedia.org/wiki/Demographics_of_New_York_City

[Demographics-of-Toronto-Neighbourhoods]:https://en.wikipedia.org/wiki/Demographics_of_Toronto_Neighbourhoods

[Foursquare-Developer-API]:https://foursquare.com

[Boroughs-of-New-York-City]:https://en.wikipedia.org/wiki/Buroughs_of_New_York_City

[Canada-List-Postal-Code]:https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

[Geospatial-Data-of-Canada]: http://cocl.us/Geospatial_data

[Geocoder-Python-package]:https://geocoder.readthedocs.io/index.html

[BeautifulSoup-package]:http://beautiful-soup-4.readthedocs.io/en/latest/
