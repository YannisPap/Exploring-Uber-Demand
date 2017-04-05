# Exploring Uber demand in NYC

![](http://www.sharingcodes.com/wp-content/uploads/2014/08/uber-new-york-map-713x330.png)

## Summary  

The dataset I used for this project included data of Uber cars' ridership in the city of New York for the first six months of 2015. As I was exploring it, I noticed that, against my initial intuition, the weather variables had not any or very weak impact on the ridership.  
Going further in my analysis it was getting more clear that the demand follows specific patterns both during the day and during the week.  
Also, I noticed a general trend of rising demand during the six months, led the total demand from 2,000 pickups per hour to 3,500.  

Using the above conclusions I was able to model the demand with forecasting horizons from a week to next hour. These models can be used in different occasions. For example someone could use the weekly forecasting model to have a general view of the next week's demand. On the other hand, a real time system could compare the prediction per borough, with the positions of Uber cars and highlight the areas accordingly to drivers' applications helping them to roam more efficiently through the city.  

Since the model is based on past observations it is prone to wrong estimations on very irregular conditions. Additionally since current observations affect future prediction, demand out of the ordinary levels may lead to wrong estimation at some point to later predictions.  

(**Note**: *This is a brief report of the results. Also available, the full analysis ([HTML](https://yannispap.github.io/Exploring-Uber-Demand/) / [Markdown](https://github.com/YannisPap/Exploring-Uber-Demand/blob/master/exploring_uber_demand.md)) and the [R Notebook](https://github.com/YannisPap/Exploring-Uber-Demand/blob/master/exploring_uber_demand.Rmd).*)  

***

## Final Plots and Summary

### Plot One

![download.png](figures/Plot%20One-1.png)

### Description One
The distribution of the four major boroughs, on a square rooted scale, are mainly normal to bimodal because of the quick rise of the demand during the morning hours.  
Staten Island's pickups follow a geometric distribution because of the very small demand in the area.  
Finally, on EWR the demand is practically zero with a very few pickups that we may consider as outliers.

***

### Plot Two

![plot2.png](figures/Plot%20Two-1.png)

### Description Two

On the above heat maps we can see the demand pattern on each borough.  
The four major boroughs follow the same pattern both during the day and through the week.  
On working days the demand falls after midnight and then at around 6 o'clock start rising quickly, then it hits a plateau during the afternoon and then rises again during the evening/night. On the X axis (during the week), the demand starts low on Monday and then rises until Saturday, when it tops and then on Sunday starts falling again. The pattern is more obvious on Manhattan and Brooklyn.  
On the two minor boroughs, Staten Island's demand looks random during the day but again we can see that the demand slightly rises as we move through the week. EWR, as we noted before has practically no demand.

***

### Plot Three

![plot3.png](figures/Plot%20Three-1.png)

### Description Three

I concluded the Exploratory Data Analysis process with the creation of some models to predict the demand. In general, the models have a very good fit with just one occasion of underestimating the actual demand on the highest day of the six months period.
