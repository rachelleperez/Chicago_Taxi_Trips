# What affects a taxi ride in Chicago? (An analysis for hypothetical ride-sharing company Zuber)

### Background

This project is part of the Data Scientist training program from Practicum by Yandex. More info in link below:

https://practicum.yandex.com/data-scientist 

### Project Setup

You're working as an analyst for Zuber, a new ride-sharing company that's launching in Chicago. Your task is to find patterns in the available information. You want to understand passenger preferences and the impact of external factors on rides.

You'll study a database, analyze data from competitors, and test a hypothesis about the impact of weather on ride frequency.

**Skills Used: Data Collection and Storage (SQL)**

### Data Description

*A database with info on taxi rides in Chicago:*

**neighborhoods table: data on city neighborhoods**
* name: name of the neighborhood
* neighborhood_id: neighborhood code

**cabs table: data on taxis**
* cab_id: vehicle code
* vehicle_id: the vehicle's technical ID
* company_name: the company that owns the vehicle

**trips table: data on rides**
* trip_id: ride code
* cab_id: code of the vehicle operating the ride
* start_ts: date and time of the beginning of the ride (time rounded to the hour)
* end_ts: date and time of the end of the ride (time rounded to the hour)
* duration_seconds: ride duration in seconds
* distance_miles: ride distance in miles
* pickup_location_id: pickup neighborhood code
* dropoff_location_id: dropoff neighborhood code

**weather_records table: data on weather**
* record_id: weather record code
* ts: record date and time (time rounded to the hour)
* temperature: temperature when the record was taken
* description: brief description of weather conditions, e.g. "light rain" or "scattered clouds"


### Conclusion

A new ride-sharing company **Zuber** is looking to launch in Chicago, IL (USA). As an analysr for Zuber, I have been tasked with answering "What Affects a Ride?" by finding patterns relating to passenger preference and the impact of external factors on rides. 

After analyzing a public data sample of taxicab trips from November 2017 and weather reports, the following insights were discovered: 
* **Flash Cab is the most successful taxicab company in Chicago** doing almost double the trips as the next company (Taxi Affiliation Services). Due to its overwhelming success, Zuber should consider looking more closely into what this company is doing to achieve such success, perhaps by hiring a consultant with domain experience in the local cab industry. In addition, Zuber should recruit drivers from Flash Cab for its service as they will come in 'Flash Cab' branded cars which due to its popularity might be more trusted.
* Although Chicago cabs can be any color, **taxi  use color strategically to be better identified** (or perhaps to be identified with successful competitors) which became evident as many used it as part of branding in their name and particularly relied on the "yellow" color (a natural choice due to its popularity in other cities and its origin in Chicago).  If possible, Zuber should recruit drivers with taxi cab colors identified with more reputable companies (like Blue/white for Flash Cab or the recognized yellow if others).
* Although Chicago boasts over 90 distinct neighborhoods, **most trips end in the Loop area or surrounding within Downtown Chicago**. Zuber could consider going head to head with these companies in that area or perhaps an even better opportunity of trying to encourage customers outside this area to use Zuber as assumingly they might not be serviced well by the current system. 
* **Weather plays a significant effect on trip duration with bad weather days yielding longer duration for the same trip**. As longer trips lead to cabs being busy in their trips longer and less supply. Zuber must consider the effect on weather on pricing. Should there be a "bad weather" surcharge? Should charge be based on duration so they end up being more expensive on bad weather days? 

### Technologies Used

* Python (Pandas, Numpy, MatPlotLib, Seaborn, Scipy)

