# Weather Data Visualization
## Project Description
Weather Data of record high and record low temperatures over a 10 year period is plotted for each calendar day. An overlay scatter plot shows the record break in the temperature in the following year. The visualization gives useful insights into the data such as, variation in maximum and minimum temperature over the months and the record breaking hottest and coldest days of the year. 

## Data Resource
Data is collected from [Daily Global Historical Climatology Network](https://www1.ncdc.noaa.gov/pub/data/ghcn/daily/readme.txt) (GHCN-Daily). The GHCN-Daily is comprised of daily climate records from thousands of land surface stations across the globe.
 
The Weather data is for Ann Arbor area near Michigen United States. It consists of a time period ranging from 2005-2015. The data comes from various weather monitoring stations installed at different locations. Each data row corresponds to a single observation of weather data for a single day from one station. The data columns represent station ID, Date, Temperature Value and Element variable which has two possible values 'TMAX' and 'TMIN' representing weather the data reading is for maximum or minimum temperature recorded for the day.

The data consists of 165k rows.

## Methodology

1. **Preprocessing Data:**  Some data prepocessing is required to bring the data in required form. First temperature data values are divided by 10 since they are given in tenths of values. Leap dates are dropped for the purpose of visualizing the data.
2. **Splitting Data:** Data needs to be split into two time periods. First, 10 year time period from 2005 to 2014 and second, 2015 for making an overlay scatter plot of record break. Each dataset will be split further based on maximum temperature and minimum temperature values recorded in a day. 
3. **Grouping Data:** To find the record high and record low for a given calender day over the 10 year period the data will be grouped by calender day and the maximum and minimum temperature for that day will be extracted. For the year 2015, the data will be grouped in the same way and then it will be compared with the 10 year data to see if any record is broken for a given calender day. 
4. **Visualizing Data:** Finally, the data is visualized by making line plots for record high and record low temperatures for all 365 calender days. An overlay scatter plot is made to show any record that is broken in 2015 for a given calender day.

## Insights 

A viewer can see the trend in weather data really easily that would have been very hard to spot just by looking at data in tabular form. 

1. July is the hottest month of the year where record temperature has reached close to 40 degree celsius. The record low temperature in July is still the highest than the record low temperature of rest of the months. 

2. January and February are coldest months of the year where record temperature dropped close to -30 degree celsius. 

3. In 2015, many 10 year records of record highest and lowest temperature have been broken.

3.1 In February, temperature dropped below -30 degree celsius, which was the lowest temperature ever recorded in the 11 year period of (2005-2015).

3.2 Many days in 2015 were the hottest days compared to the previous record of 10 years.

3.3 Many days in February were the coldest days compared to the previous record of 10 years. 
