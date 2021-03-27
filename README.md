# PyBer_Analysis
# Overview of the analysis: 
* V. Isualize, from a ride-sharing application, PyBer, has assigned us the task of creating a summary DataFrame of the ride-sharing data by city type. Using Python, Pandas, and Matplotlib, we will perform an analysis that shows the fares for each city type. The analysis will display the total ride count, total driver count and total fare amounts, as well as the average fare per driver and ride. We will compare the differences between these values to assist and advise PyBer on business decisions. 

# Results:
![Summary Data] https://github.com/BBBrian1124/PyBer_Analysis/blob/challenge/Challenge/Analysis/Summary%20Data%20Frame.PNG
* From our analysis, we generated a DataFrame that shows the total # of rides, drivers and fares along with the average fare per ride and driver. As expected, when looking at this, we see that where there are more rides, there are more fares collected. However, despite the total fares increasing as the number of rides increase, the average fare per ride and driver decrease. This is partly explained by the fact that there are more rides and drivers.

![Drivers to Ride Count] https://github.com/BBBrian1124/PyBer_Analysis/blob/challenge/Challenge/Analysis/%23_drivers_rides.png
* However, if we take look at this simple chart, it shows that in urban city types, the # of driver far exceeds the # of rides, whereas in rural and suburban city types, the ride count exceeds the driver count. In supply and demand terminology, this means that in urban cities, we have a larger supply (number of drivers) than we have demand (number of rides). Generally speaking, when supply exceeds demand, this has a negative impact on price, which may be why we see a decrease in the average fare per ride and driver (as perhaps we have to charge a lower fare/rate).

![Drivers to Ride Count - Avg Fare per Ride] https://github.com/BBBrian1124/PyBer_Analysis/blob/challenge/Challenge/Analysis/DriveRidesRatio_AvgFareRides.png

![Drivers to Ride Count - Avg Fare per Driver] https://github.com/BBBrian1124/PyBer_Analysis/blob/challenge/Challenge/Analysis/DriveRidesRatio_AvgFareDrivers.png
* A look at a scatter plot which shows the number of drivers on the x-axis and number of rides on the y-axis can also help visualize this. The size of the circles represent the average fare per ride and driver (respectively). The scatter plot shows that where the number of drivers exceed the number of riders, the average fare price per ride and driver is less in comparison to where the number of drivers and rides are around the same amount. Logically, this makes sense since, in a ride sharing service, we wouldn't want a one to one relationship. In other words, each driver should be providing multiple rides. When the driver count exceeds the ride count, this suggests that there may be drivers who are idle or not generating income.

![Total Fare by City Type] https://github.com/BBBrian1124/PyBer_Analysis/blob/challenge/Challenge/Analysis/Total_Fares_by_City_Type.png

![Total Rides by City Type] https://github.com/BBBrian1124/PyBer_Analysis/blob/challenge/Challenge/Analysis/Total_Rides_by_City_Type.png
* One way we can try to assess the "success" of each city type (i.e. we can consider this a business unit or division) is by comparing the percentage breakdown of total fares and total rides. We should expect that the percentage breakdown is similar, when comparing the two, as that would suggest that our 'input' (i.e. # of rides provided) correlates with our 'output' (i.e. total fares or revenue). This appears to be the case at PyBer, as visualized by these pie charts.

# Summary:
* Based on the above analysis, there is more information that needs to be gathered to perform further analysis to address some potential concerns. 
* We see that in that from rural to suburban to urban cities, the average fare per driver decreases by 29% from rural to suburban then 58% from suburban to urban. This combined with the fact that we have more drivers than rides in urban cities suggests that PyBer should assess whether this many drivers are needed. Additionally, seeing as the percentage breakdown in total fare and total rides are similar, this suggests that having more drivers available doesn't correlate to more fare (i.e. revenue). In other words, there is a diminishing return, where the additional drivers may not be providing more value. 
* First: further analysis needs to be done to as to whether the additional drivers provide other sorts of value. For example, if having more drivers available results in less wait time for riders, or less wasted travel time from one rider to the next due to wider coverage. These can be considered value-added services which can be factored in to the rate/price charged to the rider/customer, therefore we need to assess whether they are truely value-added or not.
* Second: the distance or time for the trips should be tracked. This would allow us to perform analysis on fare per distance travelled or time spent which is a better comparison (since we would be comparing the same units) rather than just per trip (which can vary in distance and time spent). By tracking this metric, we can use this analysis to guide pricing/rates (i.e. rate per distance, or per time, or a combination to account for traffic) and determine inefficiencies (i.e. we only generated "$y" fares for "x" distance or time).
* Third: tracking rides by driver ID as well can also provide further insight. If the driver ID is linked to the ride, we can track how many rides each driver provides to better manage our "resources". Under the assumption that PyBer (and ride-sharing applications) compensate "employees" (i.e. the driver) on a commission basis, with the driver ID linked to each ride, along with the metrics above, PyBer can adjust their compensation accordingly. For example, if having idle drivers waiting is a value-added service, we can charge more to the customer, and pay out a portion of that to the driver, or provide a small fixed salary, whereas a compensation structure like this would not make sense if they are not adding value.

# Appendix 
[Repository Link] https://github.com/BBBrian1124/PyBer_Analysis/tree/challenge/Challenge

[Code File] https://github.com/BBBrian1124/PyBer_Analysis/blob/challenge/Challenge/PyBer_Challenge.ipynb
