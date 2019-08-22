---
layout: post
title:  "The Battle of Neighbourhood - Report"
date:   2019-08-15 20:34:49 +0100
categories: report update
---

## 1.0 Introduction 

### 1.1 Statement of the Problem 
Mujaware Services LLC wants to open (restaurant) business but doesn't know which one of these two neighbourhoods, the Manhattan and the Downtown in the New York City and the Toronto City respectively, is better to open or cite a company or business. 
Hence the problem is
how to determine the right neighbourhood for Mujaware Services LLC to open a (restaurant) business.

### 1.2 Research Questions
To solve the above-mentioned problems, the right research questions should be: 
* are there relevant data on these two neighbourhoods of concern - the Manhattan and the Downtown Neighbourhoods in the Toronto and the New York Cities respectively with sufficient characteristics?
* What features (variables) or characteristics that can influence or affect a choice of neighbourhood?
* Does the available data have enough characteristics or features e.g proximity to market, population, labour force, water, transport facilities, raw material, climate, site and others that are  factors to be considered in citing a business?
* is the Downtown neighbourhood of the Toronto City better than the Manhattan neighbourhoods of the New York City in citing a business or vice versa?
* finally, which neighbourhoods is the best to be recommended to the company's stakeholders?

### 1.3 Aim (Goal)
The goal is to recommend the best neighbourhood between the two given neighbourhoods to the company stakeholders and other interested audience at large.

### 1.4 Objectives
The stepping stones towards achieving the earlier mentioned goal are:
* one, to collect the relevant data that best represent both neighbourhoods and highly likely to provide solutions to the problem.
* two, to explore and analyse the promising dataset.
* finally, to come up with solution to the earlier problem and communicate the findings and make recommendations to the relevant audience or the company using story-telling. 

### 1.5 Audiences (Stakeholders)
The right audience for this work is the Mujaware Services LLC's management and other people who may want to cite or start up a business in the neighbourhooods earlier-mentioned.

### 1.6 Significance (Justification) of the Study
The project or solution is important to the stakeholders and other audiences  because it provides the best  neighbourhood to be considered in citing a business in the city.
Besides, it helps the audience or stakeholders in making or reaching decision quickly. 

### 1.7  Background (Literature Review)

Muware Services LLC is service-rendering company that has been in existence for several years. This year, the management of the company is planning of expanding their services to one of the two cities' neighbourhoods of the New York City and the Toronto City. 

The New York City and the Toronto city are both cities in different countries United States and Canada respectively. The two respective neighbourhoods that is of interest here are the Manhattan in the New York City and and the Downtown in Toronto.

[Nytha (2019)] [Nytha-K-C-2019] found that the New York City is seven times larger than the Toronto City in term of neighbourhoods and amenities.

[Muhammad (2019)] [Muhammad-2019] found that the following:

the Downtown Toronto have only historical place while monument or landmark venues is in Manhattan. Besides airport facility, harbor, sculpture garden and boat or ferry services are available in Downtown Toronto while the Manhattan has venues like night life, climbing gym and museums. The Downtown Toronto and the Manhattan neighbourhoods are more similar in venues but less dissimilar in venues and facilities.

[Nytha (2019)] [Nytha-K-C-2019] found the following:

the Manhattan is the busiest area in New York City having lots of amenities. The New York City and Toronto City have more dissimilarities than similarities. You can find more offerings or services in New York than Toronto City which implies many factors which you can assume like high cost of living, more transport facilities, more people, ethnicity, etc. The New York City have more night life than the Toronto City. Most of the happenings are in the Downtown of Toronto.

[Khan (2019)] [Khan-2019] found that the Toronto City seems to have more uniform neighborhood type than New York City and the later has much more varieties.

[Khan (2019)] [Khan-2019] found the following:

"The Manhattan has by far the highest average income as well as population density than other boroughs. Other four are poorer.
For Toronto, population density is slightly higher in the Old City of Toronto and York than the other three. In terms of Average income, Old city of Toronto has highest average income but not very far from other four.
Toronto has much more uniform distribution of population and average income than the New York City".

Hence, based on observation and the available data before analysis, the hypothesis or assumption is that 
the Manhanttan neighbourhood of the New York City is better to be recommended to the audience than the Downtown neighbourhood of the Toronto City.

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

## 3.0 Research Methodology/Materials/Tools

### 3.1 Tools / Materials
The tools or materials mainly used in the research are:
* Numpy library
* Pandas library 
* Matplotlib library
* Folium library 
* Foursquare API
* Machine learning library (Scikit-learn library).

### 3.2 Methods
The methods used in this project are:
* Collection techniques,
* Data pre-processing techniques 
* Data preparation techniques 
* Data analytical techniques 
* Data visualization techniques 
* Inferential statistical testing techniques (machine learning technique e. g K-means clustering)

### 3.3 Research Design 
The blueprint of this research starts with:
*	One, collection of relevant data from the available open-sourced datasets.
*	Two, literature review of the past works on the subject matter which guide the researcher on the choice of data, variable or properties and method used in this research.
*	Three, data analysis of the sample of data obtained from the dataset.
*	Finally, statistical testing of the data using the machine learning algorithm – the K-mean clustering.

### 3.3   Data Collection Techniques
The data requirements as specified earlier were reviewed and followed to obtain the initial dataset from the aforementioned sources of data for this project. The datasets collected or downloaded were scrutinized using pandas library based on the data requirements to make sure conditioned met before moving to the next stage.
### 3.4   Data Analytical Techniques
#### 3.4.1 Exploratory Data Analysis
The data sets of the two neighbourhoods, the Downtown and the Manhattan were visualized to gain knowledge of the distribution of variables and the neighbourhoods in the Boroughs, the Downtown and the Manhattan, using folium library to see how the neighbourhoods in this borough are spatially distributed. The resulting data is subjected to initial step of data analysis – the exploratory data analysis (EDA) to gain insight on how correlated or trending the data are.
After the data sets have been subjected to exploratory data analysis using Folium, Seaborn and Matplotlib libraries to see how the variables of the data are distributed, trending and insight gained, the data was then subjected to pre-processing stage.
#### 3.4.2     Data Pre-processing
The resulting data sets were checked for data integrity. The missing values of the data addressed and erroneous or irrelevant attributes of the data expunged using Pandas library. Thence the data were formatted where the categorical values or variables of the venues returned by the Foursquare API were converted to numeric values through one hot encoding using a method from the Pandas library

#### 3.4.3   Data Preparation
The relevant attributes of the data are retained after pre-processing and selected. The selected attributes or features' data types checked and corrected. After the categorical variables of the data converted to numeric form using one hot encoding method from Pandas library and transformed into the desired state, then it was then being subjected to inferential statistical testing.

### 3.5    Inferential Statistical Testing Techniques (Machine Learning)
Here the encoded data during the analysis are fed into the machine learning algorithm - K-mean Clustering - to group or segment the neighbourhoods. At the end, the neighbourhoods that have similar characteristics are grouped together. Thence the similarities and dissimilarities of the Downtown and the Manhattan are observed. 

you introduce the research methods and data sources you used for the analysis. If you have collected new data, explain the data collection exercise in some detail. 
You will refer to the literature review to bolster your choice for variables, data, and methods and how they will help you answer your research questions.

## 4.0 Results
### 4.1 Data Analysis
### 4.1.1 Descriptive Statistics
Table 1: First Five of Group of Neighbourhoods and Venues of the Manhattan
![Manhattan Groupby](/images/manhattan-groupby.JPG){:class='img-responsive'}

The result obtained when the Manhattan neighbourhoods are grouped shows there are 341 uniques venue categories in the Manhattan as shown in the table 1 above. The first five neighbourhoods in the table do not represent this number above but the rest of the neighbourhoods can be viewed here(link). Note that, this result returned by the Foursquare API is within the radius of 500.

Table 2: First Five of Group of Neighbourhoods and Venues of the Downtown
![Downtown Groupby](/images/downtown-groupby.JPG){:class='img-responsive'}

Also, the result obtained when the Downtown neighbourhoods are grouped shows that there are 207 unique venue categoies in the Downtown as shown in the table 2 above. The first five neighbourhoods returned by the Foursquare API in the table do not represent this total but the rest can be viewed here.(link) Also, note that, the returned result is within the radius of 500. 

Table 3: The Most Common Venues of the First Five Neighbourhoods of the Downtown
![Downtown Venues](/images/downtown-venues.JPG){:class='img-responsive'}

When the Downtown neighbourhoods is analysed, the resulting distribution of the venues associated with the respective neighbourhoods in the Downtown is shown above on the table 3. Here in the Downtown there are 1284 venues as returned by the Foursqure API which are within the radius of 500 metres

Table 4: The Most Common Venues of the First Five Neighbourhoods of the Manhattan
![Manhattan Venues](/images/manhattan-venues.JPG){:class='img-responsive'}
Likewise, when the Manhattan neighbourhoods is analysed, the resulting distribution of the venues associated with the respective neighbourhoods in the Downtown is shown above on the table 4. Here also in the Manhattan, there are 3324 venues as returned by the Foursqure API which are also within the radius of 500 metres

Table 5: First Five Cluster Neighbourhoods of the Downtown
![Downtown Cluster](/images/downtown-cluster.JPG){:class='img-responsive'}

When the Downtown Borough is analysed and clustered, the resulting 10 most common venues and cluster labels associated with the various neighbourhoods are shown in the table 5 above.

Table 6: First Five Cluster Neighbourhoods of the Manhattan
![Manhattan Cluster](/images/manhattan-cluster.JPG){:class='img-responsive'}
Again, when the Manhattan Borough is analysed and clustered, the resulting 10 most common venues and cluster labels associated with the various neighbourhoods are shown in the table 6 above.

Figure 1: The Downtown's Map Showing Neighourhood and Venues
![Downtown Venues Map](/images/downtown-venues-map.JPG){:class='img-responsive' width='1440px'}

The figure 1 above shows distribution of the neighbourhood and venues in the Downtown Borough  when they are superimposed on the map of Downtown Toronto. This map represents the distribution before being clustered


Figure 2: The Manhattan's Map Showing Neighourhood and Venues
![Manhattan Venues Map](/images/manhattan-venues-map.JPG){:class='img-responsive' width='1440px'}

Besides, the figure 2 above shows distribution of the neighbourhood and venues in the Downtown Borough  when they are superimposed on the map of the Manhattan Borough. This map represents the distribution before being clustered

### 4.2 Testing Hypothesis Result
When the neighbourhoods of the two Boroughs are clustered into 5 groups using machine learning algorithm - K-mean Clustering - the resulting clusters of neighbourhoods in borough are shown below in figure 3 and 4 below.

Figure 3: The Manhattan's Map Showing Neighourhoods and Venues' Clusters
![Manhattan K Mean](/images/manhattan-kmean.JPG){:class='img-responsive' width='1440px'}

When the neighbourhoods and venues of the Manhattan Borough are superimposed on the map of Manhattan after being clustered, the resulting distribution of the neighourhoods and venues are shown above in the figure 3.

Figure 4: The Downtown's Map Showing the Neighbourhoods and Venues' Clusters
![Downtown K Mean](/images/downtown-kmean.JPG){:class='img-responsive' width='1440px'}

Similarly, when the neighbourhoods and venues of the Downtown Borough are superimposed on the map of Downtown after being clustered, the resulting distribution of the neighourhoods and venues are shown above in figure 4.



## 5.0 Discussion
### 5.1 Observations
The Manhattan has about 341 unique neighbourhoods categories. The venues in this place are 3324. The Downtown Toronto has about 207 unique neighbourhoods categories. The venues in this neighbourhood are 1284.
The important venues in the Manhattan neighbourhoods are:
* Financial District 
* Grocery Store 
* Bank 
* Building 
* Bus Station 
* Business Services 
* College and Academic Building
* Farmers market 
* Restaurant
* Financial and Legal Services 
* Food Court 
* Hotel 
* Waterfall 
* Residential Building and others not but shown in the table 2.4


The important venues also in the Downtown neighbourhoods are:
* Airport Services 
* Bank
* Restaurants 
* Building
* College 
* Farmers market 
* General Entertainment 
* General Travel
* Hospital
* Hotel 
* Market 
* Train Station 
* Trail 
* And others not mentioned here but shown on the table 2.5

To cite a business, many factors involved in the location of individual industries are availability of raw materials, water, labour, markets, capital, efficient management, the transport facilities, site, insurance facilities, government policies, and climate and power resources.

The question is does the data sets have these characteristics mentioned to address the problem or the research question. Though the data sets do not 
have these features directly yet we could infer these properties indirectly from the foursquare geolocation data like venues in the two neighbourhoods. 

The two neighbourhoods in the Manhattan of the New York City and the Downtown Toronto of the Toronto City - are similar in having banks, grocery, market, farmers market, waterfall, college, transport station and buildings but dissimilar in other venues listed above and in the table 2.5 shown above in the result section.

These venues that are similar indirectly represent availability of capital made available by bank, raw materials provided by the farmers markets and groceries, water provided by waterfall, labour provided by the colleges and the universities, efficient management provided by the college and the competitors which are in the restaurant businesses in the neighbourhoods, transport facilities provided by the presence of bus or train stations in the neighbourhoods.


### 5.2 Comparison
The data sets used in this research are similar to the ones used in the previous researchers on these neighbourhoods. The result here tells us what factors should be considered in citing a restaurant business in either of the two neighbourhoods and inferred the factors from the available neighbourhoods and venues in the two neighbourhoods.

### 5.3 Disagreement
The previous researches used socio-demographic and socio-economic features or characteristics particularly population and average income that are not available for the Downtown Toronto but the Manhattan datasets. These were used to come up with solution to their research problems and questions. The solutions to the problem should have been based on factors that influence the decision of citing a business in area. 

### 5.4   Findings
The result of this research provides more logical answers to the research questions and problems by inferring the characteristics of the data sets that influence the citing of restaurant business in either the Manhattan or the Downtown Toronto from the venues and activities associated with the neighbourhoods in the two area of interest. These make us to relate the number of venues in the neighbourhoods of the Downtown (207) and the Manhattan (342) to the population and hence the market shares of any potential restaurant business to be cited. So the number of venues likewise the population or population density in the Downtown is less when compared with the Manhattan. As such the market share of any prospective restaurant business in the Manhattan will be more than that of the Downtown Toronto.

### 5.5 Recommendations
Even though there are factors that are not available during the research, the research still recommend that the Manhattan neighbourhoods should be considered in citing a restaurant business if the two boroughs given to be considered are the Manhattan and the Downtown.

*Explain results/present explanation of the result
*Compare with existing or past works.
*Justifications for disagreements/differences with earlier works should be made. 
The discussion section is where you rely on the power of narrative to enable numbers to communicate your thesis to your readers. You refer the reader to the research question and the knowledge gaps you identified earlier. You highlight how your findings provide the ultimate missing piece to the puzzle.
Of course, not all analytics return a smoking gun. At times, more frequently than I would like to acknowledge, the results provide only a partial answer to the question and that, too, with a long list of caveats.

## 6.0 Conclusion

### 6.1 Summary
In the end, the Manhattan neighbourhoods are better than the Downtown neighbourhoods in citing a restaurant business based on the available data. Why? Though the two neighbourhoods are similar in factor that influence the location of restaurant business yet they are glaringly dissimilar in the population densities and hence the market shares of a potential restaurant business.
Any potential restaurant businesses cite in the Manhattan will have large market share because of the population or population density of the area than if it is to be cited in the Downtown. 

### 6.3 Challenges
The obvious challenges recorded during the research work is insufficient data on the variables or factors that influence the decision of citing a restaurant business in either the Manhattan or the Downtown Toronto of the New York City and the Toronto City respectively. 

### 6.4 Future Development
As soon as the researcher comes across a worthy or significant data that are characterized by variables or features that influence the citing of business the two neighbourhoods of interest, this work will be revisited to test our findings or generalization.

### 6.5 Future Application
Besides if the sufficient data sets of the right characteristics or factor are found and the earlier assertions are revisited, the application of the findings will be of great importance to any prospective investors, stakeholders or capitalists who want to situate a restaurant business or any related business in the two borough - the Manhattan and the Downtown Toronto. 

In the conclusion section, you generalize your specific findings and take on a rather marketing approach to promote your findings so that the reader does not remain stuck in the caveats that you have voluntarily outlined earlier. You might also identify future possible developments in research and applications that could result from your research






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
