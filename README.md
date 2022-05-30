# PyBer_Analysis

## Overview of the Analysis

This analysis examines a Pyber ride sharing dataset that includes data for 2,375 rides in 120 service areas, from January 1, 2019 to May 8, 2019. The ride observations include a ride ID number, the date/time, the fare, and the service area. The service area (called cities in the dataset) data includes the city name, number of drivers, and the service area category (urban, suburban, rural). The analysis develops summary statistics to allow comparisons across the three service area categories. 

## Analysis of Ride Sharing Statistics Across Service Area Categories

The analysis generated a summary data frame (see link below) with the following statistics:
https://github.com/benniehana111/PyBer_Analysis/blob/main/analysis/Pyber%20summary%20dataframe.png

Total # of Rides
Total # of Drivers
Total Fares (in $US)
Average Fare  (in $US)
Average Fare per Driver (in $US)

These statistics indicated that there are more drivers and more rides in urban areas, and the fewest drivers and rides in rural areas. They also indicate that average fares lowest in urban areas and highest in rural areas. These statistics my suggest that ride sharing is cheaper and more available in urban areas (and expensive/less available in rural areas), but more data is required to prove this hypothesis.

The analysis also provides a line graph showing total fares by service area type from January 1, 2019 thru April 29, 2019. This graph shows that most of Pyber's revenue comes from urban areas, and that there was a drastic reduction in ride sharing in urban and suburban service areas for several days around April 1st.

## Summary

The available data is insufficient to provide actionable insights for Pyber. I recommend the following corrective steps:

1) Change the existing naming convention of "city" to "service area." Reporting data for urban, suburban, and rural cities don't make sense.

2) Better ride data - PyBer should use GPS signals to collect the following additional data fields for each Ride ID:
    Driver ID
    Distance traveled
    Elapsed time
    
This data is needed to allow PyBer to observe differnces in driver utilization and ride sharing travel patterns across service areas.
    
3) Better service area data - PyBer should use online/archival research to collect the following data for every service area:
    Population density
    Road density
    Traffic intensity
    
This data is needed to control for driving environment conditions across service areas.

4) Macro travel patterns - PyBer should collect an additional data field from GPS signals; the startpoint and endpoint of each ride (by service area). Detailed analysis of this data (possibly including creation of GIS overlays) should be conducted to observe to what extent rides travel across - or entirely outside - Pyber's existing service areas.

This analysis is needed to determine whether or note the current service areas are useful units of analysis, or if different geographic units of observation are needed to understand PyBer's operations.
