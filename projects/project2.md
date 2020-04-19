# Project 2 | GES 486 | Alicia Sabatino
## Project Description
This project aims to analyze the spatial shift of incarceration hot spots in the United States from urban to rural and suburban areas. This project uses data from the 1970s to the 2010s. This spatial shift is well documented and investigated in scholarly research, but surprisingly under-mapped. 
## Data Description
I used data from the United States Census Bureau (link) and the Vera Institute of Justice for this project. The Vera Institute of Justice compiled an Incarceration Trends dataset, which is freely available on their github page (link).  These datasets are not spatial and unprojected, so I used the GEOIDs from each dataset to link to a 2019 TIGER/Line Counties (and equivalent) shapefile. This file was reprojected to the pseudo-mercator projection for the final web maps.
## Analysis
### Data Transformation
This data was transformed using R. I wrote scripts to subset the data to make it more easy to manipulate, analyze, and use with GIS applications. I isolated the columns I needed for this project, and then saved separate files for each 5 year increment. I also saved a file with the desired columns with all years for graphing purposes. 

### Analysis Tools
To create graphs and summary tables I used R and Excel. These graphs show the 
## Products 
### Current Products
First, I created a map showing the counties designated as four categories: urban, small/mid sized metropolitan area, suburban, and rural. 

(insert map)

I created a time-lapse map showing the shift in incarceration trends by five year increments. 

(gif)
## Future Products
In project 3 I hope to use this data to compare prison and jail capacities to hospital capacities. I hypothesize that rural counties that have experienced an incarcerated population boom, financed by the U.S. government, do not have adequate healthcare facilities.  I hope to produce more graphs and interactive maps to illustrate where the shift was largest, and possibly investigate other factors that correlate with the largest shifts from urban to rural incarceration. 
