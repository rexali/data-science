---
layout: post
title:  "The Battle of Neighbourhood!"
date:   2019-05-23 05:16:49 +0100
categories: report update
---

## 1.0 Introduction 

### 1.1 Statement of the Problem 
Mujaware Services LLC wants to open (restaurant) business but doesn't know which one of these two neighbourhoods - the Manhattan and the Downtown in the New York City and Toronto City respectively - is better to open or cite a branch of the company or business. 
Hence the problem is
how to determine the right neighbourhood for Mujaware Services LLC to open or start up a (restaurant) business.

### 1.2 Research Question and Hypothesis
To solve the above-mentioned problems, the right research questions should be: 
* are there relevant data on these two neighbourhoods of concern - the Manhattan and Down Town Neighbourhoods in the Toronto and New York Cities respectively with sufficient characteristics?
* What features (variables) or characteristics that can influence or affect a choice of neighbourhood?
* Does the available data have enough characteristics or features e.g proximity to market, population, labour force, water, transport facilities, raw material, climate, site etc that are  factors to be considered in citing a business?
* is the Downtown neighbourhood of the Toronto City better than the Manhattan neighbourhoods of the New York City in citing a business or vice versa?
* finally, which neighbourhoods is best to be recommended to the company's stakeholders?

Hence, based on observation and the available data before analysis, the hypothesis or assumption is that 
the Manhanttan neighbourhood of the New York City is better to be recommended to the audience than the Downtown neighbourhood of the Toronto City.

### 1.3 Aim (Goal)
The goal is to recommend the best neighbourhood between the two given neighbourhoods to the company stakeholders and other interested audience at large.

### 1.4 Objectives
The stepping stones towards achieving the earlier mentioned goal are:
* one, to collect the relevant data that best represents both neighbourhoods and highly likely to provide solutions to the problem.
* two, to explore and analyse the promising dataset.
* finally, to come up with solution to the earlier problem and communicate the findings and make recommendations using to the relevant audience or the company using story-teling. 

### 1.5 Audience (Stakeholders)
The right audience for this work is the Mujaware Services LLC's management and other people who may want to cite or startup a business in the neighbourhooods earlier-mentioned.

### 1.6 Significance (Justifications) of the Study
The project or solution is important to the stakeholders and other audiences  because it provides the best  neighbourhood to be considered in citing a business in the city.
Besides, it helps the audience or stakeholders in making or reaching decision quickly. 

### 1.7  Background (Literature Review)

Muware Services LLC is service-rendering company that has been in existence for several years. This year, the management of the company is planning of expanding their services to one of the two cities' neighbourhoods of the New York City and the Toronto City. 

The New York City and the Toronto city are both cities in different countries United States and Canada respectively. The two respective neighbourhoods that is of interest here are the Manhattan in the New York City and and the Downtown in Toronto.

The New York City is seven times larger than the Toronto City in term of neighbourhoods and amenities. ([Nytha K. C., 2019] [Nytha-K-C-2019])

Downtown Toronto have only historical place while monument or landmark venues is in Manhattan. Besides airport facility, harbor, sculpture garden and boat or ferry services are available in Downtown Toronto while the Manhattan has venues like night life, climbing gym and museums. The Downtown Toronto and the Manhattan neighbourhoods are more similar in venues but less dissimilar in venues and facilities. ([Muhammad, 2019] [Muhammad-2019])

Manhattan is the busiest area in New York City having lots of amenities. The New York City and Toronto City have more dissimilarities than similarities. You can find more offerings or services in New York than Toronto City which implies many factors which you can assume like high cost of living, more transport facilities, more people, ethnicity, etc. The New York City have more night life than the Toronto City. Most of the happenings are in the Downtown of Toronto. ([Nytha K. C., 2019] [Nytha-K-C-2019])

The Toronto City seems to have more uniform neighborhood type than New York City. The later has much more varieties. ([Khan, 2019] [Khan-2019])

"The Manhattan has by far the highest average income as well as population density than other boroughs. Other four are poorer.
For Toronto, population density is slightly higher in the Old City of Toronto and York than the other three. In terms of Average income, Old city of Toronto has highest average income but not very far from other four.
Toronto has much more uniform distribution of population and average income than the New York City". ([Khan, 2019] [Khan-2019])

## 2.0 Data 
### 2.1 Data Requirements
The dataset or set of data available for this project are:
* Demographics of New York City from U.S. Census of 2000, the New York Department
of city planning hosted by [N Y U] [Demographics-of-New-York-Census]
* Demographics of New York City from wikipedia page - [Demographics of New York City] [Demographics-of-New-York-City]
* List of Postal Codes of Canada from wikipedia - [Canada List Postal Code] [Canada-List-Postal-Code]
* Boroughs of Nework City from wikipedia - [Boroughs of New York City] [Boroughs-of-New-York-City] 
* Demographics of Toronto Neighbourhoods from wikipedia which is in turn taken from 2006 Canadian Census - [Demographics of Toronto Neighbourhoods] [Demographics-of-Toronto-Neighbourhoods]
* Foursquare API Geolocation data - [Foursquare API] [Foursquare-Developer-API]

The New York City's neighbourhoods dataset for this project is collected from '2000 New York City Neighborhood Names' dataset hosted by NYU’s Spatial Data Repository.
The addresses of the neighbourhoods got from the dataset are used to obtain their equivalent latitude and logitude coordinates of each neighbourhood using geocoder API.

Similarly, Toronto's neighbourhoods data are collected or scraped from the Wikipedia page, [Canadian List of Postal Code] [Canada-List-Postal-Code], wrangled, cleaned, then read into a pandas dataframe and structured and formatted like the New York dataset.

The other datasets are to be visualized and drawn an information or insight from them to complement the anlaysis.

The Foursquare API is to be used to acquire data neighborhoods in New York City and Toronto city in terms of common venues and its categories in each neighborhood, and then use these feature to group the neighborhoods or segment(cluster) them.
Foursquare describe a ‘venue’ as a place that one can go to, or check-in.
The Foursquare ‘venue’ is assigned a ‘category’ and each ‘category’ is given a ‘categoryID'



### 2.2 Data Understanding
The data collected based on the data requirements above. The dataset is opened source dataset. 
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
the Longitude is an imaginary line running north and south of Green Wich meridian measured in numeric.
The borough is a subset of city. The neighbourhood is the community area name. 

The target value (variable) or label of the data set is the neighbourhood which is the dependent variable. The other variables is like longitudes, latitudes, venues, etc are the independent (predictor) variables.





<!--
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}
-->

<!--
Check out the [Canada List Postal Code][Canada-List-Postal-Code] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Geospatial Data of Canada][Geospatial-Data-of-Canada]. If you have questions, you can ask them on [Geocoder Python package][Geocoder-Python-package].
-->


[Khan-2019]: https://www.galibhassankhan.com/2019/04/10/segmentation-and-comparison-of-neighborhood-toronto-new-york-using-foursquare-api-and-clustering/

[Muhammad-2019]: https://capstoneprojectreport.blogspot.com/2019/01/the-battle-of-neighborhoods.html?m=1

[Nytha-K-C-2019]: https://starnithi.blogspot.com/2019/01/the-battle-of-neighborhoods.html?m=1

[Demographics-of-New-York-Census]: https://www1.nyc.gov/site/doh/data/health-tools/neighborhood-statistics-demographics.page

[Demographics-of-New-York-City]:https://en.wikipedia.org/wiki/Demographics_of_New_York_City

[Demographics-of-Toronto-Neighbourhoods]:https://en.wikipedia.org/wiki/Demographics_of_Toronto_Neighbourhoods

[Foursquare-Developer-API]:https://foursquare.com

[Boroughs-of-New-York-City]:https://en.wikipedia.org/wiki/Buroughs_of_New_York_City

[Canada-List-Postal-Code]:https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

[Geospatial-Data-of-Canada]: http://cocl.us/Geospatial_data

[Geocoder-Python-package]:https://geocoder.readthedocs.io/index.html

[BeautifulSoup-package]:http://beautiful-soup-4.readthedocs.io/en/latest/
