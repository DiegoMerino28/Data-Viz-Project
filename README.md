# Airline on Time Performance Exploration
## by Diego Merino

## Dataset
We'll be using a Dataset from the Bureau Of Transportation statistics that records information about flights in the US, the delays associated and the reason for those delays.

Main dataset: https://www.transtats.bts.gov/DL_SelectFields.aspx?gnoyr_VQ=FGJ&QO_fu146_anzr=b0-gvzr
Auxiliary datasets: https://community.amstat.org/jointscsg-section/dataexpo/dataexpo2009

We've performed the following wrangling:
* Dropped canceled or diverted flights.
* Dropped flights that arrived early or just on time.
* Also, we dropped the data points with more than 500 minutes since we're not interested in flights that are delayed more than 8 hours, that can be seen as a rare occurence.
* We joined the data with two auxiliary datasets with information about the carriers and airports.


## Summary of Findings

* We found that the main factor for delays was carrier induced delays. 
* Airlines that have a bigger volume of flights tend to have more delays.
* There's a negative correlation between distance flown and delays.
    * This can be explained due to Operating factors. As a plane flies more legs on one day, delays tend to accumulate.
* Following on the last point, we checked the difference between short, medium and long haul flights. We observed the same relationship.
* We also found that, the bigger the airline, the more skewed to bigger delays they are.
* 95\% of the arrival delays are explained by departure delays, meaning that rarely a flight is delayed more on arrival than on departure.
* The other 5\% is mainly explained by National Air System Delays, which can be due to saturation in arrivals, meteorology-led deviations from routes etc. 

## Key Insights for Presentation

* Airlines are the main factor that explain delays in the US. 
* 95\% of the arrival delay is explained by the departure delay.
* Hubs are the main pain point for Airlines.

