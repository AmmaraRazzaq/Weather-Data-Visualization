# Weather-Data-Visualization
## Project Description
Weather Data of record high and record low temperatures over a 10 year period is plotted for each calendar day. An overlay scatter plot shows the record break in the temperature in the following year.

## Data Resource
Data is collected from [Daily Global Historical Climatology Network](https://www1.ncdc.noaa.gov/pub/data/ghcn/daily/readme.txt) (GHCN-Daily). The GHCN-Daily is comprised of daily climate records from thousands of land surface stations across the globe.
 
The Weather data is for Ann Arbor area near Michigen United States. It consists of a time period ranging from 2005-2015. The data comes from various weather monitoring stations installed at different locations. Each data row corresponds to a single observation of weather data for a single day from one station. The data columns represent station ID, Date, Temperature Value and Element variable which has two possible values 'TMAX' and 'TMIN' representing weather the data reading is for maximum or minimum temperature recorded for the day.

The data consists of 165k rows.

## Methodology

1. **Preprocessing Data:**  Some data prepocessing is required to bring the data in required form. First temperature data values are divided by 10 since they are given in tenths of values. Leap dates are dropped for the purpose of visualizing the data.
2. **Splitting Data:** Data needs to be split into two time periods. First, 10 year time period from 2005 to 2014 and second, 2015 for making an overlay scatter plot of record break. Each dataset will be split further based on maximum temperature and minimum temperature values recorded in a day. 
3. **Grouping Data:** To find the record high and record low for a given calender day over the 10 year period the data will be grouped by calender day and the maximum and minimum temperature for that day will be extracted. For the year 2015, the data will be grouped in the same way and then it will be compared with the 10 year data to see if any record is broken for a given calender day. 
4. **Visualizing Data:** Finally, the data is visualized by making line plots for record high and record low temperatures for all 365 calender days. An overlay scatter plot is made to show any record that is broken in 2015 for a given calender day.

