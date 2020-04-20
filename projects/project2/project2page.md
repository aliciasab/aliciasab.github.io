# Project 2 | GES 486 | Alicia Sabatino
## Project Description
This project aims to analyze the spatial shift of incarceration hot spots in the United States from urban to rural and suburban areas. This project uses data from the 1970s to the 2010s. This spatial shift is well documented and investigated in scholarly research, but surprisingly under-mapped. The vera institute produced an online tool to show their data, but this tool did not investigate rural v. urban trends in incarceration.

## Data Description
I used data from the [United States Census Bureau](https://www.census.gov/developers/) and the Vera Institute of Justice for this project. The Vera Institute of Justice compiled an Incarceration Trends dataset, which is freely available on [their github page](https://github.com/vera-institute/incarceration_trends).  These datasets are not spatial and unprojected, so I used the GEOIDs from each dataset to link to a 2019 TIGER/Line Counties (and equivalent) shapefile. This file was reprojected to the pseudo-mercator projection or Albers for the final web maps. 
## Analysis
### Data Transformation
This data was transformed using R. I wrote [scripts](add.link) to subset the data to make it more easy to manipulate, analyze, and use with GIS applications. I isolated the columns I needed for this project, and then saved separate files for each 5 year increment. I also saved a file with the desired columns with all years for graphing purposes. 

### Analysis Tools
To create graphs and summary tables I used R and Excel. Graph 1 shows the pre-trial incarceration rate increases as a whole over the years, meaning the number of people incarcerated who aren’t convicted has significantly increased through time. Graph 2 shows pretrial incarceration rates / 100,000 people by density classification. This shows an increase in rural incarceration through time.
(graph 1) (graph 2)

## Products 
### Current Products
First, I created a map showing the counties designated as four categories: urban, small/mid sized metropolitan area, suburban, and rural. 

(insert map)

Maps 2 and 3 show county level incarceration rates per 100,000 people in 1975 and 2015. The most striking thing on these maps is the overall, nearly uniform increase in incarceration rates around the country. 

(insert maps)

I created a time-lapse map showing the shift in incarceration trends by five year increments from 1975 - 2015. 

(gif)

## Future Products
In project 3 I hope to use this data to compare prison and jail capacities to hospital capacities. I hypothesize that rural counties that have experienced an incarcerated population boom, financed by the U.S. government, do not have adequate healthcare facilities.  I hope to produce more graphs and interactive maps to illustrate where the shift was largest, and possibly investigate other factors that correlate with the largest shifts from urban to rural incarceration. I can estimate the number of beds from other data points, like prison capacity and prison population.
I also hope to work with this (prisons in R,) just couldn’t get it to work yet. 
https://www.gl-li.com/2018/02/05/map-prisons-in-the-united-states/
I would also like to make better graphs.
Note: of the top 100 counties with the highest incarceration rates in 2015, a vast majority, if not all were rural.
