# GIS-Day-Project
**Analyzing Workforce Area Characteristics around transportation hubs in New York City**


**Topic:** 
This project was a competition entry for NYU's GIS Day that was held on 18th November 2015. 

**Tools used:**
ESRI ArcMap, MS Excel, Tableau (Bar chart generation)

**Idea:**
Are jobs in New York City scattered at random, or is there any pattern to it based on the backbone of the city, its transportation? 
This project aims to understand if there is a specific pattern in the nature of jobs located around transportation hubs (NYC subway stations in this case) or not.

**Data:**
LEHD Origin Destination Employment Statistics is a census dataset that provides data on employers and employees, such as number of jobs based on age, ethnicity, industry, race, etc. This data is provided at a block level, based on place of work and residence per census block. Data used for this project is based on place of Work (Workforce Area Characteristics) and is initially obtained for the whole state of New York for the year 2013. The file used was 'ny_wac_S000_JT00_2013' indicating WAC data for all jobs in NY state in the year 2013. In order, to filter the data to represent only NYC, a geographic crosswalk file, also provided with the data is used. URLS for the data source, as well as the cleaned and merged data file (wac_nyc) used for analysis is provided in the 'Cleaned Data' folder.

Also, to visualize the data a basemap of New York City census blocks is used. Subway stations are plotted on the basemap as points. Urls for obtaining these shapefiles are provided in the 'Cleaned Data' folder.

**Approach:**

1. I collected the LEHD data for New York State and then cleaned it to limit the data only to New York City, using MS Excel. 

2. This data was then merged with the Census Block data and plotted on ArcMap software along with the Subway Station locations. 

3. I then did a buffer analysis around each subway station with a buffer distance of 0.25 miles (equivalent to 3 city blocks). 

4. The next step was to find the most populous industry for each workplace block, and then narrow down the 20 industry categories types to the top 9 categories for the sake of plotting on the map. The most populous industry (industry with maximum employees) per block was determined using MS Excel formulas.

5. The distribution of those categories for boroughs of NYC are captured as well (except for Staten Island since they do not have subway lines). 

6. Following this, I made a count of each industry category within and beyond the buffer and plotted it on a bar chart.

**Result:**
Based on the analysis performed, the industries with considerably more number of employees *AROUND* subway stations are 'Accomodation and Food Services' and 'Retail Trade'.
Also, the industries with considerably more number of employees in the census blocks *AWAY* from subway stations (in the area outside buffer regions) are 'Construction' and 'Wholesale Trade'.


This map was awarded the Second Prize for Poster Maps among 16 entries in that category.
