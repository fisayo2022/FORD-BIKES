# Cogo Ride Exploration and Visualization 2022
## by Fisayo Sofuwa


## Dataset

The [Cogo Bike](https://en.wikipedia.org/wiki/CoGo) Share system launched in July 2013 with a network of 300 bicycles and 30 stations located throughout downtown Columbus. Today, CoGo boasts around 90 stations and 600 bikes serving Columbus, Bexley, Upper Arlington, Grandview Heights and Easton. The system provides Columbus residents and visitors an additional transportation option for getting around town that is fun, easy, and affordable. 

CoGo is available for use 24 hours a day, 365 days a year and includes both classic pedal bikes and electric assist ebikes. The station network provides twice as many docking points as bicycles, assuring that an available dock to return your bicycle is always nearby. [here](https://cogo-sys-data.s3.amazonaws.com/index.html)

>**N.B**: The data used for this exploration is data from **`January`** to **`August`**.

##### Data wrangling process:
- fix started_at and ended_at not in correct format to datetime datatype.
- Missing values start_station_id, start_station_name, end_station_id and end_station_name, and end_lat and end_lng.
- Drop unnecessary columns(ride_id, start_station_id, end_station_id).
- Create a trip duration column from started_at and ended_at.
- Create trip start date, trip start hour of the day, day of the week and month
- cast 'start_dayofweek' to category dtype.
- cast 'start_month' to category dtype for easy plotting.


## Summary of Findings

The number of trips peaked around 15-19pm with saturday been higher than other days. For the 2022, between January to August, the ride service usage increases with month except for almost same usage for January and February, and for fall in July and August. Most riders are casuals and ride type are classic bike. Most rides were quick and short, lasted between 4 to 13 minutes. There was no unusual points and no transformation was also needed due to straightforwardness of the data.

There are a lot of member than casual users and the riding habit varies alot between both user type. Members and casuals uses the bike sharing system for work commute thus having low average trip between on work days (Mon-Fri) whereas casual tends to ride for fun especially over the weekend. 

There are lot more member usage than casual overall. The short and efficient period of usage  for member between Monday through Friday indicate the use primarily for work commute. The more higher and flexible pattern of casual use shows that they are taking advantage of the bike sharing system quite differntly heavily over the weekends for city tour or leisure purposs probably.


>**N.B**: The data used for this exploration is data from **`January`** to **`August`**.

## Key Insights for Presentation

Different usage pattern/habit between the two type of riders are seen from the exploration. Members and casuals use the bike sharing system heavily on work days i.e. Monday through Friday whereas casual users rides a lot on weekends, especially in the late afternoon through evening. Many trips concentrated around 15pm-19pm on work days for members, while customers tend to use it more over the weekend with small difference between member and casual usage. The efficient/short period of usage for members corresponds to their usage from Monday to Friday, indicating the use is primarily for work commute. The more relaxing and flexible pattern of causual users shows that they're taking advantage of the bike sharing system quite differently from members, heavily over the weekends for city tour or leisure purpose probably.