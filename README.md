<img src="https://www.emagister.com/assets/es/logos/centro/id/136150/size/l.jpg" alt="logo ironhack" style="width:150px;height:100px;">

# GeoSpatial Data



## Table of Contents

- [Project Description](#project-description)
- [Database & API](#database)
- [Workflow](#workflow)
- [Results](#results)
- [Organization](#organization)
- [Conclusions](#conclusions)
- [Links](#links)

## Project Description
Welcome to our gaming company! We believe that a good cup of coffee and freedom are essential for creativity, growth and innovation. Our commitment to designing games that inspire joy and imagination, creating a positive and inclusive community, and prioritizing the health and well-being of our team members guide everything we do. Join us on our journey to create meaningful and impactful games that bring people together.

As we prepare to open a new office, we want to ensure that our space reflects our values and meets the needs of our team members.

* __Encouraging learning and sharing:__ Our designers enjoy attending design talks and sharing knowledge. 
* __Supporting families:__ 30% of our team members have at least one child. 
* __Fostering innovation:__ Our developers prefer being around successful tech startups that have raised at least $1M. 
* __Promoting well-being:__ Our executives are big fans of Starbucks, and our CEO is a vegan. 
* __Supporting travel:__ Our account managers travel frequently. 
* __Creating a fun and engaging environment:__ Everyone in our company is between 25 and 40 years old. 
* We also need a __basketball court__ about 10 km away for the maintenance guy and ensured there's a __pet groomer__ nearby for our office dog, "Dobby."



## Database & API
__Mongo__ database containing information from startups around the world was used as the database for this project. 

__Foursquare__ was used as an API to find places that fit the team's needs. Foursquare is a location data platform that provides API access to millions of venues, points of interest and other location-based data. 


## Workflow

![wf](/images/workflow.jpg)

01. First, we analyzed the need of our employees and developed a __weighting table__ to identify the most important factors.

02. We then __queried the database__ to determine the cities where the highest revenue video game companies are located and we selected San Francisco, New York and Santa Monica as reference points.

03. Since we value inspiration and want to be close to the tech and design environment, we located the __approximate coordinates__ near tech startups with less than 100 employees that had raised over $1,000,000 in funding rounds.

04. Next, we used the __Fourquare API__ to identify locations and spaces that met our team's needs within a maximum radius of 2,000 meters from our approximate coordinates.

5. Finally, we __mapped all the locations__ found for each city using Folium and developed a final weighting table based on the number of locations and their distance to the center. This helped us determine which of the three cities met all of our requirements with the shortest distance.

## Results
![cat](/images/categories.jpg)

01. San Francisco *(white marker)*
* __Latitude__: 37.787872
* __Longitude__: -122.403612
* __Country__: United States
* __City__: San Francisco
* __Street__: 110 Kearny St
* __Postal Code__: 94108
* __Landmarks__: Transamerica Pyramid, Union Square, Chinatown district

![sf_map](/images/sf_map.jpg)

02. New York *(white marker)*
* __Latitude__: 40.748782, -73.986534
* __Country__: United States
* __City__: New York City
* __Street__: 22 W 34th St.
* __Postal Code__: 10001
* __Landmarks__: Madison Square Garden, Empire State Building, Chelsea neighborhood, * __Broadway theater district

![ny_map](/images/ny_map.jpg)

03. Santa Monica *(white marker)*
* __Latitude__:  34.019858
* __Longitude__: -118.492769
* __Country__: United States
* __City__: Los Angeles (near Santa Monica)
* __Street__: 1334 Lincoln Blvd
* __Postal Code__: 90035
* __Landmarks__: Westfield Century City mall, Los Angeles County Museum of Art, Beverly Hills High School

![sm_map](/images/sm_map.jpg)

## Organization
<u>Notebooks</u>
 * __Mongo__: to perform queries on the startup database and identify the three cities and relevant tech companies and create dataframes with this information.
 * __Four Square (4sq)__: to find locations that met our team's needs and create dataframes with this information. 
* __Folium__: to create maps for each city to visualize our findings.

<u>Data</u>
 * __Tech companies__: CSV format dataframes. One for each city.
 * __Four Square (4sq)__: CSV format dataframes. One for each city.
 * __City maps__: HTML format maps</u>: One for each city.

<u>Images</u>
* Included images for the README document to help illustrate the process and findings.


## Conclusions
After evaluating the three candidate cities, Santa Monica has been discarded as it does not meet our requirements, as the points of interest for our employees are too dispersed across the map within a 500m radius. Between San Francisco and New York, a new weighting table was created to determine which city better meets our needs.Finally, NEW YORK is the city that best meets our needs in terms of smaller surface area and distance. San Francisco offers similar resources, but they are more dispersed. 

However, there are some requirements that we were unable to meet, such as proximity to an airport. Being located near an airport would proportionally decrease the distance to other points of interest. Despite this, the closest airport is LaGuardia Airport (LGA), which is 17 miles away by car or 35 minutes away by public transportation according to Google Maps.
![ny_airport](/images/ny_airport.jpg)
In conclusion, after a detailed evaluation of the candidate cities, we have decided to establish our new headquarters in New York, specifically in the Midtown South neighborhood. We believe that this location will provide the best resources and convenience for our employees while meeting our business needs. Although we were unable to fulfill all of our requirements, we are confident that this location will provide the best overall solution for our company. We are waiting for you!

![ny_center](/images/ny_center.jpg)
![ny_center_zoom](/images/ny_center_zoom.jpg)


## Links
[API - 4sq](https://foursquare.com/)



