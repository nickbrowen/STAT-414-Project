# STAT-414-Project

## What I did:
### Eric
##### Merging
I think the merge is complete. We have two new data files: 

1. `final_data.csv` is data on each athlete, with NA values included for each of the EV's we are considering. We can use this file to do some more cleaning if we decide to omit or include any of the EV's.
n = 1973

2. `final_data_noNA.csv` is the data on each athlete with NA values omitted. We will probably end up using this file for EDA.
n = 1368

##### Tidying
I cleaned the "Result" variable which recorded the time athletes finished their time in. It was formatted differently for different years and events, and it was a stubborn character type. It is now two new variables.
* `timeSecs` is the time in seconds. Type is numeric.
* `timeMins` is the time in minutes. Type is numeric.

*Note:* I had to remove long distance events like the marathon, 20km walk, and 50km walk because the times were obviously wrong. Many of the finishing times for marathon had vague, incorrect values like "35:15:10". Obviously nobody medaled in the marathon by finishing in either 35 minutes or 35 hours. Enough of these wierd values were present that I just removed these events.

##### EDA
I made a couple of quick plots but I didnt have much time. Just wanted to look at the relationships between a couple of variables quickly.


### Nick


## To do next:
Start the EDA

##
Okay, so I removed all the strictly non-running events (ie hurdles, steeple chase) and also changed the event to a numeric measure of distance. (dataset = track) This should allow us to have only 2 levels with athlete and country. I'm still working on getting all the output together. Also, can you see my updated files? I'm not sure if I'm doing it right