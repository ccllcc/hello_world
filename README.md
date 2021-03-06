# Make effective data visulization
## Summary

The dataset I used for this project is found on Kaggle, containing air quality information (AQI) of main Chinese cities from 2010 to 2015. I used the data for Shanghai to explore the impact of differnet weather conditions to the air quality. In this project, I've dived further into the relationship between wind speed(Iws) vs air quality(AQI).

Finding of the visualization:\
Overall\
We witness that there is a similar pattern of the index trend through a year: the winter is always worse than summer. The worst record was taken at end 2013 and almost reached 400.

Yearly View\
This chart shows with more details the year to year AQI comparison. In 2012, we see almost each season AQI surpass 150. In 2013, the air pollution got even worse compared to 2012. 2015 was the best year with control and attention as except the beginning and end of the year, from March to October, not a day higher than 100.

Wind Speed vs AQI\
This is a scatter plot, to show the correlation of wind speed again air quality index. We can witness that all the points with value greater than 100 on the x axis are less than 200 on the y axis. This shows that the bigger the wind speed, the less chances getting a high value. The correlation is negative.

Wind Direction vs Wind Speed vs AQI\
In this chart, the wind direction has been brough into the chart to produce a 3 dimensional chart to reveal further the complexity and correlations. From the chart, we could tell that when the winds come from SE(south east), the AQI appear to be within the lowest range(<=120). When the winds come from NW(north west) or there is no wind movement, the AQI could go above 200. And it appears that the winds from north move faster than those from south.

Seasonality\
When split the scatter plot by season, it also reveals some interesting findings: it confirms the finding in line plot, that summer is the best season of air quality in Shanghai. If you want to visit this city, the best choice will be summer.(personal recommendation) You could also choose autumn, but some of the days could be polluted. Winter is the worst among all year.

## Design

Originally I have made line chart to show the AQI trend along the year as the date information is available in the dataset, hence a line is perfect to show a data set with date dimension and could reveal transition. I used the scatter plot to reveal the bi-variable (wind speed Iws vs air quality AQI) correlation. After receiving the comments, I added animation, and color encode to the line charts and scatter plot. 

A diverging color pallette to the scatter plot was to draw readers attention, as red shows that the index is the worst among the filtered data points, and green is the best among filtered data points. 

I've involved further dimension into the charts by leveraging animation to bring more vivid comparison.

## Feedback to the original design
#### What do you notice in the visualization?
Person A\
I see a line representing the AQI along year 2015 and it was starting from March that this index got stablize, which was less than 100. Again starting from Nov, the index got increased and surpassed 100. Is it possible to show more comparison across year and season?(to original design)\
Person B\
I also see for the scatter plot, the horizontal axis is air quality index and vertical axis is wind speed. I understand that the red color means that the air quality is bad and green means the air quality is good. My understanding was confirmed when hovering onto each of the data point.(to original design)\
Person A\
I can not see clearly the yearly trend, all mixed up.(to the intermediate design)\
Person C\
I like the color pallette used for the scatter plot, which draws me my attention to the values of the data points.(to the original design)

#### What questions do you have about the data?

What's the granularity of the data used in this project?
What's the source of this dataset?

#### What do you think is the main takeaway from this visualization?

I hope if it is possible, to see a year by year comparison, and it is already good to have the yearly pattern.
If there any more correlation could be explored via the scatter plot?

#### Is there something you don’t understand in the graphic?
Nope...

## About the Data Set
The data set was originally found on Kaggle. There are two data sets are used for generating the charts in ShanghaiPM_final.html and ShanghaiPM_origin.html. 'PMShanghai_2015.csv' was used for the original html to scratch some ideas and also used for the scatter plot in the final html. 'PMShanghai_daily.csv' was used to generate the line chart.

## Resources
https://developer.mozilla.org/en-US/docs/Web/CSS {grasped CSS basics}\
https://developer.mozilla.org/en-US/docs/Web/HTML {grasped html basics}\
https://github.com/PMSI-AlignAlytics/dimple/wiki {where I went through the basic dimple functionality}\
https://www.health.ny.gov/environmental/indoors/air/pmq_a.htm {where I get some background knowledge about PM2.5}\
https://www.kaggle.com/ {where I found my dataset}
https://airnow.gov/index.cfm?action=aqibasics.aqi {Air Quality Index basics}
http://www.csgnetwork.com/windspeedconv.html {Wind speed units reference}
