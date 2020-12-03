# 2008 Flight Statistics in US
## by Shu Liu


## Dataset

> The dataset I used for this project reports flights in the United States during the year of 2008 with 7,009,728 records in total, including carriers, airports, arrival and departure delays as well as flight cancellations. The data source along with description of data fields can be found [here](http://stat-computing.org/dataexpo/2009/the-data.html). By analyzing this data set, I'm trying to answer the following questions:

* In 2008, what are the numbers of flights operated by each carrier and at each airport
* What is the busiest month during the year and the busiest hour during a day?
* How much are flight delayed on average by each carrier at each hour?
* What are the primary reasons for flight delays by each carrier?

## Summary of Findings

* Observation 1:
> DepDelay and ArrDelay look to have a very strong positive relationship, which indicates if the more a flight is delayed at departure, the more likely that arrival will be delayed and vice versa. There is also somewhat positive relationship between number of total flights and cancellation. Though this trend isn't as obvious as the relationship between arrival and departure delay time.

* Observation 2:
> There isn't a clear relationship between arrival/depature delay and number of flights. I think this is because different airports have different levels of capability to handle flight traffic. Thus less number of flights at an airport doesn't necessarily mean less cases of flight delays.

* Observation 3:
> United Airlines has the longest average departure delays, and American Airlines has the longest average arrival delays. On the opposite side, flights with Aloha Airlines are advanced on average. I took a further look and it turns out more than 75% of the time Aloha Airlines fly planes earlier than CRS schedule.

* Observation 4:
> From 6AM to 8PM there is a gradual increase in the average departure delay time per hour. I think this is because if there are flights delayed in the previous hour, the flight departure schedule in the next hour will be disrupted as a result. So the flight delay situation will aggregate over time. Then during midnight hours since airports generally schedule less flight departure, the trend does down evetually. There is a similar trend for the arrival time, yet the arrival delay trend is lagged compared to the departure delay trend. I believe this lag is in alignment with time it takes for a plane to fly between two locations.

## Key Insights for Presentation

* Insights 1: At what hour do people mostly likely to experience the worst flight delays?

> Overall, AM flights experience less delays than PM flights for both departure and arrival.

> From 6AM to 8PM there is a gradual increase in the average departure delay time per hour. I think this is because if there are flights delayed in the previous hour, the flight departure schedule in the next hour will be disrupted as a result. So the flight delay situation will aggregate over time. Then during midnight hours since airports generally schedule less flight departure, the trend goes down evetually.

> There is a similar trend for the arrival time, yet the arrival delay trend is lagged compared to the departure delay trend. I believe this lag is in alignment with time it takes for a plane to fly between two locations. Additionally, flight arrival around 6-7AM tend to be earlier than scheduled.

* Insights 2: What's the biggest reason for departure delay at each airport?

> For most of airline companies, the two biggest reasons for flight delay are late aircraft and NAS (national air system) delay. On the other hand, for airline companies like Comair, Mesa Airlines and Atlantic Southeast Airlines, the top two reasons are carrier delay and weather delay.

> In general, very few delays are caused by security reasons. Appreciate the hardwork by security screening officers!