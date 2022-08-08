# Squirrels in NYC

## Story Summary

Do Squirrels make New Yorkers pause and take a breath?

The idea for collecting this data was thought up by Jamie Allen, when he realized that the research surrounding the common Eastern gray squirrel did not exist. It was simply overlooked.

This story would be written as a mental check, by bringing attention to something people pay no attention to -squirrels. The meaning of the story can also be extrapolated to other life things. The story on the squirrels has already been done, but the story/angle on the squirrel’s relationship to people has not. A lot of New Yorkers encounter squirrels everyday but may not even register that they do. And for the individuals that do subconsciously notice the squirrels, how much thought are they really having when it comes to what they are seeing?  In a city like New York City, where the culture is fast-pasted and has individuals functioning like a well-oiled machine, how many people “stop to smell the roses” or appreciate the little things? Has the same squirrel been following you or is it a different one? (The data can give us a pretty good idea, but can you?)

The data shows that the squirrels are not running away from people the busier the park is. This means they should be visible. Do New Yorkers notice the squirrels? The data also shows, on average, there are more squirrel sightings per min in Central Manhattan, but Upper Manhattan has the most squirrels per acer of park. Meaning that the New Yorkers, assuming they are still moving like they’re-on-a-mission, are more likely to encounter a squirrel in the parks of Central Manhattan then they would be if they passed through Upper Manhattan; even though Upper Manhattan is found to have more squirrels per acre. 

## Sourcing

In this project, I analyzed [“Park Data”](link_here) and [“Squirrel Data”](link_here) from the Squirrel Census sourced from NYC Open Data, along with [“Parks Properties”](link_here) data from NYC Open Data. I joined all these data sets into one workbook to analyze their elements. 

### Potential Interview Contacts
1) Denise Lu, graphics editor at The New York Times
	* Email: denise.ds.lu@gmail.com
	* Denise Lu was one of the volunteers that helped count he squirrels in central park for the squirrel census. She also reported on the process and the findings. I would like to know her experience and interest in this data. As a New Yorker herself, has she ever taken time to think about the squirrels before? I’d also like to know the feedback she got on her reporting on the Squirrel Census. What are the overall feelings on this data?
2) Jamie Allen, creator of the Squirrel Census
	* Email: jameswilliamallen@gmail.com
	* Jamie Allen is the creator of the Squirrel Census and a write along with multimedia creator. I’d like to know from him why he felt like the squirrel census needed to be created. Just because there is a gap of missing information doesn’t necessarily mean that the world needs that information, so why squirrels? Why the Squirrel Census? How does he feel about the squirrels being overlooked? Were there any other motives, aside from science, behind the creation of the squirrel census?

### Additional Sources

1) The Squirrel Census [“Stories”](https://www.dropbox.com/s/dwjrjo6omoum754/stories.csv?dl=0) data sheet.
	* This source provides descriptive elements of the surrounds/happening when the data was collected. It also indicates which area and park name these observations came from.
	* This source can be used to grasp a general environment of the location in which the squirrels appear and what is happening at that time. Do people seem to notice or are they wrapped up in something else? It gives a third person perspective/observation on the everyday New Yorkers.
 
2) National Geographic article [“How many squirrels live in NYC’s Central Park? We finally have the answer”](https://www.nationalgeographic.com/animals/article/squirrel-census-new-york-city-central-park)
	* This source provides information related to the squirrel census data and history/insight on the squirrel community. 
	* This source can be used to introduce the data and connect it back to the community. It identifies “who cares” about the squirrel data. This also demonstrates general New Yorker mentality when it comes to more frivolous information like squirrel data. Its sources can act as opposing opinion potentially. 

## Data Visualization

### [Colors of Squirrels in NYC](https://datawrapper.dwcdn.net/4C9wj/2/)
![choropleth](https://github.com/sofiaschmidt/j124-final-project/blob/2a032bf3d3ab97b2d050aa3486b5c3a1ffb29730/screenshots%20for%20data/graph001.png)

## Data Analysis Process
The first step I took was to clean my data sets. The data sets that I was using did not need much cleaning at all. I then combined the three data sets into one workbook in order to cross reference data.

### Scope of Analysis 

1) How many squirrels are there per acre of park in each area of New York City? Which Area of New York City has the most squirrels per acre of park?
2) Do the parks’ conditions affect the squirrels’ level of interaction with humans? 
3) Which park type attracts the most amount of squirrels? Which park type attracts the least amount of squirrels?
4) Do certain color squirrels prefer certain precincts?
5) Varying times were spent in each park observing the squirrels; for the purpose of normalizing the data, how many squirrels were seen per minute in each area of the city?

### Analysis
1) How many squirrels are there per acre of park in each area of New York City? Which Area of New York City has the most squirrels per acre of park?

First, I determined the acreage of each park by using a pivot table I created from ‘park-info’ dataset. This data is organized by properties, so some parks have multiple entries.

Then, in the ‘park data’ sheet I added a column labeled “acres” and used vlookup (including wildcard keys to help the search) to get the value from the park-acreage data.

Next (because some names did not popup), I added a new column labeled “search name” to help the search. I manually searched for names in the ‘park-info’ dataset and updated the search name so that vlookup can find the data.

<img width="468" alt="img001" src="https://github.com/sofiaschmidt/j124-final-project/blob/2a032bf3d3ab97b2d050aa3486b5c3a1ffb29730/screenshots%20for%20data/img001.png">

> (data results here)
