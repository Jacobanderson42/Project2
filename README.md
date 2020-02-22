# Project2
Project 2 for B ME 450\
GitHub repository link\
GitHub code link

# Problem Statement
This project was looking to analyze the data taken by the meteorology instrument package. We look to be able to plot the wind speed and 
rain rate for each location while differentiating between times of windy and rainy. We also look to find the cross correlation between 
the two sites and what the lag between the data of each location is. A plot of the monthly average of rain and wind is also created for 
each of the locations.

# Background/Solution/Results
The meteorology instrument package is used to measure weather conditions on the sea surface. The sensor measures wind speed in the north 
and east directions as well as the total amount of rain. The rain data is taken as a measurement of the total rain in a self siphoning 
tube. This means that the tube fills up with rain and once the device is full it empties the water inside. In order to find the rate of 
rainfall, the difference in the total water measurement over a period of time must be calculated. Additionally, to find the total wind 
speed, the north and east wind speeds must be added as vectors. In order to analyze the data taken by the meteorology instrument 
package, a python code was written, taking in csv files of the data, through a github link, and analyzing data in order to create graphs 
to represent the data.

The data is first downloaded from the OOI website and uploaded to github in order to allow direct access. The data is then loaded into 
colab through the github link. The data is then separated into the time, east wind velocity, north wind velocity, and total rainfall. 
This data is then analyzed to find the date, total wind velocity, and rain rate. A color is also assigned to each point based on the 
magnitude of the wind and rain values to determine whether it is windy and/or rainy at that time.

Plots are then created for both the wind and rain at each location over the time of the data. A cross correlation is then calculated for 
the wind and rain between the two locations. This allows for the analysis of the lag between the two locations and how the weather 
fronts move between the locations. The average wind and rain is also calculated and plotted from the data for each location. The plots 
of wind and rain for each location, the cross correlation, and the monthly average wind and rain for each location can be seen below.

# Graphs for Wind and Rain at Each Location
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonOffshoreSurfaceRain.png)
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonOffshoreSurfaceWind.png)
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonShelfSurfaceRain.png)
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonShelfSurfaceWind.png)

# Cross Correlation Graph
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/CrossCorrelation.png)

# Graphs for Monthly Average Wind and Rain at Each Location
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonOffshoreSurfaceMonthlyRain.png)
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonOffshoreSurfaceMonthlyWind.png)
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonShelfSurfaceMonthlyRain.png)
![](https://github.com/Jacobanderson42/Project2/blob/master/Images/OregonShelfSurfaceMonthlyWind.png)

# Conclusions
It can be seen from the graphs above that there appears to be a correlation between the rain and wind between the two locations. 
Comparing the points of high wind or high rain activity shows that these peak times seem to correlate. It can also be seen in the graphs 
that the majority of the time it is not rainy regardless of if it is windy or not. Looking at the plot of rain for each location it 
appears that there is an even distribution of times when it is windy or not windy during times of high rainfall. The parameters for this 
comparison can also be changed to determine different levels of windy and rainy. For these plots, the threshold for windy times is a 
wind speed of 5m/s and a rain rate of 2mm/hr.

The cross correlation can be seen in the next plot. This shows how closely the data between the two locations are related and how much 
delay there is between the data. This delay shows the time difference of when the weather patterns hit the two instruments. This cross 
correlation shows that there is a weak correlation between the two locations. For wind the maximum correlation is .282 with a lag of 
210289 seconds. For the rain data the maximum correlation is .157 with a lag of -9617 seconds. This shows that there is likely only a 
weak correlation between the two locations. Since the max correlation is low, and the lag for the two different data sets are different 
there is not a lot of evidence to support a correlation between the two. Comparing the two cross correlations, it appears that the two 
lines follow the same general trend. This supports the idea that there is some correlation between the data at the two locations as it 
tends to change in a similar manner. This cross correlation was performed between April 1st and April 7th. These date ranges can also be 
changed to compare data at different times throughout the year. Doing so provides different cross correlation that may show more or less 
correlation between the data. This difference in correlation is likely due to the direction of movement of a weather front between the 
two locations.

In the last four graphs, the monthly average can be seen for the wind and rain at each location. The pattern of increasing wind and rain 
during the winter and spring seasons can be seen for both locations. The lowest wind and rain occurs during the summer months for both 
locations. The highest wind speed for the offshore mooring is 7.25 m/s and occured in January, and the max rain rate is .808 mm/hr this 
occured in May. The lowest wind speed for the offshore mooring is 4.29 m/s and occured in August, and the min rain rate is .486 mm/hr 
this occurred in September. The highest wind speed for the shelf mooring is 7.04 m/s and occured in January, and the max rain rate is 
1.68 mm/hr and occured in March. The lowest wind speed for the shelf mooring is 3.29 m/s and occured in August, and the rain rate is 
.411 mm/hr and occured in June.
