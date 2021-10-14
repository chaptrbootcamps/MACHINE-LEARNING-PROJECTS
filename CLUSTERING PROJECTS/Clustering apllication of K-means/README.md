# CLUSTERIGN (END WEEK PROJECT)

**Application-of-k-means**
--------

Road traffic collisions are the number one killer of young adults ages 5-29 and 8th leading cause of death worldwide. 
Post crash care is one of the five pillars of road safety and is a critical component in reducing morbidity and mortality. 
When it comes to emergency response to road accidents, every second counts. With heavy traffic patterns and the unique layout of the city, finding the best locations to position emergency responders throughout the day as they wait to be called is critical in a city like Nairobi.
(source, Flare-emergency response technologies). 

Read more updated information on causes of death [here](https://www.verywellhealth.com/top-causes-of-death-for-ages-15-24-2223960) 

![causes of death among young adults](https://www.cdc.gov/nchs/images/databriefs/1-50/db37_fig_2.png)

The data you will use has information on thousands of road traffic accidents that have occured in Nairobi in 2018 and 2019. 
Use this data to identify patterns of risks accross the city and then use this information to place six virtual ambulances around the city, moving them around throughout the data with the goal of minimizing the 
distance travelled when responding to crashes during the period under study. 

For this specific excercise you will use the K-Means clustering algorithm to find clusters of these accident occurences
then you will use your best judgement on where to position your ambulances, eg at the cluster centroids, or at the peripheries, 
constant location during the day or moving per hour, or every two hours. 
You will then use the scoring method defined below, to obtain the minimum distance. 

You must use the training data (recorded crashes up to June 2019)
The test data will be on the subsequent dates. 


**The data**

The data consists of crashes identified by the World Bank DIME research team and by Flare. ‘Train.csv’ provides time and location for 6318 crashes in the training period (2018-01-01 to 2019-06-30).
Scoring is based on the distance from each crash in the test period to the nearest ambulance (see the Evaluation section for specifics).

**Additional data is also provided:**

Weather.csv has daily weather based on the GFS dataset
Segment_info.csv contains info on specific road segments. This includes information on physical characteristics such as the existence of crosswalks or obstacles in the road as well as behavioral characteristics such as people walking along the side of the road, all of which may be associated with the likelihood of a road traffic crash. The columns have been obfuscated but the data may still be useful. It can be linked to physical locations by joining with the geometry in segments_geometry.geojson. Some segments have separate rows for each side of the road, and so two rows in Segment_info.csv may map to the same road segment in segments_geometry.geojson.
