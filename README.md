# PyBer Analysis - Module 5 Challenge
<sub>UNC Chapel Hill Data Analytics Bootcamp</sub>

## Overview of Project
For Module 5, Pandas and Matplotlib were utilized to summarize and graph the ride-sharing data from PyBer by city type. Using the given CSV files with city and ride data, the information was combined into a singular dataframe, which was then manipulated to summarize and analyze weekly fares across rural, suburban, and urban cities.

## Results
* Creating a Summary Dataframe
  * The original dataframe was used to calculate the total number of rides, total number of drivers, total amount of fares, average fare per ride, and average fare per driver for each city type. This information was then compiled into a new dataframe.

![Summary dataframe](/images/summary_df.png)

  * From this summary, it is evident that rural cities have the smallest number of both total rides and total drivers, but has the largest average fare per ride and average fare per driver. With 125 total rides and 78 total drivers, the ride-to-driver ratio is 1.6:1, leading to a higher average fare per driver. Because rural areas are, by definition, more spread out, we can assume the rides are, on average, longer than those from suburban and urban areas, leading to the higher average fare per ride.
  * Suburban rides have around 5, 6, and 4.5 times the rural total rides, total drivers, and total fares, respectively. Even so, both the average fare per ride and the average fare per driver are significantly lower than their rural counterparts. The total ride to total driver ratio is around 1.3:1, which is closer to an even 1:1 than the rural ratio. However, because it is still unbalanced, the average fare per driver stays higher than the average fare per ride.
  * Total urban rides and drivers are significantly higher than the respective results for rural and suburban rideshares, but the average fare per ride and per driver are significantly lower. The ride-to-driver ratio is around 1:1.5, showing the disproportion between the two variables, but in the opposite direction of both rural and suburban rideshares. With more drivers than rides, the average fare per driver is low. In terms of fares, urban rides can be expected to cost less than their rural and suburban counterparts - because urban areas are more compact, rides are shorter on average.
* Creating a Multi-Line Plot From the Data
  * Using the original data to create a new dataframe, rideshare data was separated by city type - rural, suburban, and urban - and by day. The dataframe was also reduced to contain dates from only January to April.

![January to April weekly dataframe](/images/jan_apr_df.png)

  * This dataframe was then plotted, creating a line graph to visualize the total fares each week from January to April.

![Total fare by city type graph](/images/jan_apr_plot.png)

  * Through visualizing the data, the differences between rural, suburban, and urban rideshare fare totals are made more apparent, allowing for at-a-glance understanding of the disparities between the city types. Patterns across rural, suburban, and urban rides are also easier to spot, such as the rise in rides in late February, followed by a swift drop.

## Summary
Although the general fare totals are likely to remain different between city types, steps can be taken to find an equilibrium between the number of drivers and the number of rides requested. Having too few drivers will make it difficult for riders to find a ride, but having too many drivers will leave some drivers without any rides, as seems to be the current case in urban areas. Looking at the average fare per ride and the average fare per driver, the current data appears to suggest that an ideal ratio of rides to drivers is roughly 1:1. For rural and suburban areas, the subsequent solution is to hire more drivers, and for urban areas, the number of drivers should be reduced. However, market studies must first be conducted in rural and suburban areas to see if the market can support more drivers.

To more accurately analyze the data, PyBer should begin collecting data on the average distance travelled per ride. This would allow a higher degree of certainty when claiming that higher rural fares are because the area is more spread out - and therefore rides are longer and cost more - and that the opposite is true for urban areas.

While using the first third of the year to observe general patterns and relationships between rural, suburban, and urban areas is beneficial, PyBer should do the same for the rest of the year, and use it as a model to determine when more or fewer drivers should be hired in order to stay consistent with customer demand. 
