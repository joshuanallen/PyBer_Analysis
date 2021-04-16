# PyBer Ride and Fare Data Analysis

Overview of the analysis: Explain the purpose of the new analysis.
Results: Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.
Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.

## Project Overview
Pyber CEO, V. Isualize, has requested an analysis of internal ride-sharing data to find disparities in drivers and fares between urban, suburban, and rural cities. V. Isualize has requested the following data:

1. An overview of below the ride-sharing data broken out into 3 categories: Urban, Suburban, and Rural 
    - total rides
    - total drivers
    - total fares
    - average fare per ride
    - average fare per driver
2. Time-series graph of the weekly fares for each city type 
3. Recommend action items based on the results of the action items

## Resources
- Data Source: ride_data.csv, city_data.csv
- Software: Python 3.7.6, Jupyter Notebook, Matplotlib, 
- References: fivethirtyeight style guide, https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.pivot.html, https://stackoverflow.com/a/19798349/15245090

## Summary

### Analysis
Picture 1.1 below shows Pyber's ride-sharing data outlining ride, driver, and fare analysis broken down for urban, suburban, and rural cities from January 1, 2019 to April 30, 2019.

**Picture 1.1** Pyber ride-sharing summary by city type
*****Insert Summary DF ******

Picture 1.2 below shows the total weekly fares collected for each respective city type from January 1, 2019 to April 30, 2019.

**Picture 1.2** Pyber total weekly fares by city type
****insert timeseries graph ***

#### Urban city type
From Picture 1.1 we see the following trends for urban cities:
- **Ride demand:** Urban city type has the **highest demand for rides** at 260% the number of rides than the suburban city type and 1300% the rural city type.
- **Driver numbers:** Urban city type has the **highest number of drivers** at 490% the number of drivers than the suburban city type and 3080% the rural city type.
- **Total fares:** Urban city type has the **highest total fares collected** at 206% the revenue of the suburban city type and 920% the rural city type.
- **Average fare per ride:** Urban city type has the **lowest average fare per ride** at only 79% of the average fare of suburban ride and 71% of the rural rides.
- **Average fare per driver:** Urban city type has the **lowest average fare per driver** at only 42% of the average fare of suburban driver and 30% of the rural driver.

From Picture 1.2 we can see that urban weekly collected fares  increased from January 2019 through Februrary 2019 and then leveled off for the remaining 2 months. March was the most volatile month in terms of positive and negative week-to-week movement.

#### Suburban city type
From Picture 1.1 we see the following trends for suburban cities:
- **Ride demand:** Suburban city type has a ride demand **500% of rural ride demand and 38% of the urban demand**.
- **Driver numbers:** Suburban city type has driver numbers **630% of rural driver numbers and 20% of the urban driver numbers**.
- **Total fares:** Suburban city type has total fares collected **450% of rural driver numbers and 49% of the urban driver numbers**.
- **Average fare per ride:** Suburban city type per ride fare average is **90% of rural rides and 126% of urban rides**.
- **Average fare per driver:** Suburban city type per driver fare average is **90% of rural rides and 126% of urban rides**.

#### Rural city type
From Picture 1.1 we see the following trends for rural cities:
- **Ride demand:** Rural city type has the **lowest demand for rides** at 20% of the suburban demand and 8% of the urban demand .
- **Driver numbers:** Rural city type has the **lowest driver numbers** at 16% of the suburban driver numbers and 3% of the urban numbers.
- **Total fares:** Rural city type has the **lowest total fares collected** at 16% of the suburban fare totals and 3% of the urban totals.
- **Average fare per ride:** Rural city type has the **highest average fare per ride** at 112% of the suburban average and 141% of the urban average.
- **Average fare per driver:** Rural city type has the **highest average fare per driver** at 140% of the suburban average and 335% of the urban average.

## Conclusions
Urban rides have lowest fares due to oversaturation of driver market or shorter distances traveled on a per ride basis. In urban areas the drivers make less per ride as the customers experience less cost on average. Total ride revenue was the lowest in January possibly due to less travel and lack of activities in urban environments after the holiday travel season.

Suburban rides are more equitable in terms of cost to user and pay for driver in that they are most aligned in the average costs per driver and per ride. Suburban fare revenues are relatively consistent week-to-week across the 4 month timeframe.

Rural rides have the highest fares due to driver scarcity or longer ride average travel distances. In rural environments users bear larger costs, but drivers may yield higher earnings per trip. Rural fare revenues are relatively consistent week-to-week across the 4 month timeframe.

### 3 recommendations for addressing disparities between city types
1. Target user acquistion in suburban and rural cities to increase revenues based on higher per ride cost, but need to match the increased user base with drivers available in those areas. Rural areas have the largest room for growth and and generating per ride revenues.

2. Encourage current urban drivers who possibly leave their home rural markets to commute and cause oversaturation in urban market. Oversaturation in urban markets can be avoided incentivizing picking up rural rides which have a higher per ride revenue than urban rides. Changing the perception that one can provide less rides and earn the same amount if they stay in a rural area with enough demand. Increasing rural driver availability can increase demand if wait time for riders/potential customers is reduced as it provides a better user experience.

3. Augment fare pricing for each demo to align pricing across the three market types to ensure drivers in all are receiving equitable pay for the same work, which encourages drivers to stay in their own market and locality decreasing urban congestion, which could potentially help with public perception of ride-sharing adoption.

### Limitations of data and script
Need larger timeframe for dataset to evaulate seasonality for demand across wider timeframe.

need wait time and demand level data for each ride to determine if driver needs are met for each city demographic.

Need ride distance data to adjust for per distance cost analysis, which can make comparison more accurate eliminating geographic differences between city types.

No data around fare rates differences within each city demo (i.e. surge pricing, discounted rates) that could affect rate data balance.

Consider using AI modeling to optimize ride availability and fulfillment and driver earnings based on demand to further this analysis. The following article outlines a process to consider: https://venturebeat.com/2020/06/24/researchers-use-ai-and-simulation-to-optimize-ride-sharing-earnings/
