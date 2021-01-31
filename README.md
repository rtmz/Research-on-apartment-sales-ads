# Research-on-apartment-sales-ads
We have the data from a real estate agency. It is an archive of sales ads for realty in St. Petersburg, Russia, and the surrounding areas collected over the past few years. We’ll need to learn how to determine the market value of real estate properties. The task is to define the parameters. This will make it possible to build an automated system that is capable of detecting anomalies and fraudulent activity.  There are two different types of data available for every apartment for sale. The first type is a user’s input. The second type is received automatically based upon the map data. For example, the distance from the city center, airport, the nearest park or body of water. 

# We'll go through the following steps:

- Open and explore files
- Process missing values 
- Convert data types 
- Calculate and add to the table: the price per square meter
- Calculate and add to the table: the day of the week, month, and year that the ad was published
- Calculate and add to the table: which floor the apartment is on (first, last, or other)
- Calculate and add to the table: the ratio between the living space and the total area, as well as between the kitchen space and the total area
- Investigate the following parameters: square area, price, number of rooms, and ceiling height
- Create histograms for each parameter 
- Examine the time it's taken to sell the apartment and create a histogram. Calculate the mean and median and explain the average time it usually takes to complete a sale. When can a sale be considered extra quick or taken an extra slow?
- Remove rare and outlying values and describe the specific details we've discovered.
- Which factors have had the biggest influence on an apartment’s value? Examine whether the value depends on price per meter, number of rooms, floor (top or bottom), or the proximity to the downtown area. Also study the correlation to the ad posting date: day of the week, month, and year. 
- Select the 10 places with the largest number of ads and then calculate the average price per square meter in these localities. Select the locations with the highest and lowest housing prices. We'll find this data by name in the ’locality_name’ column. 
- Thoroughly look at apartment offers: each apartment has information about the distance to the downtown area. Select apartments in Saint Petersburg (‘locality_name’). The task is to pinpoint which area is considered to be downtown. Create a column with the distance to the downtown area in km and round to the nearest whole number. Next, calculate the average price for each kilometer. Build a graph to display how prices are affected by the distance to the downtown area. Define the turning point where the graph significantly changes. This will indicate downtown. 
- Select a segment of apartments in the downtown. Analyze this area and examine the following parameters: square area, price, number of rooms, ceiling height. Also identify the factors that affect an apartment’s price (number of rooms, floor, distance to the downtown area, and ad publication date). 

# Description of the data
The dataset contains the following fields:

- _date_posted_ - the date the ad was posted
- _days_listed_ - the number of days the ad was listed until it was sold	
- _last_price_	- the last price of the ad
- _bedrooms_	- the number of bedrooms
- _kitchen_area_ - kitchen area in sq. meters	
- _living_area_ - living area in sq. meters
- _total_area_	- total area in sq. meters
- _balconies_ - the number of balconies	
- _ceiling_height_ - the ceiling height	
- _floors_total_	- the total number of floors in the building
- _floor_ - the floor of the apartment	
- _total_images_ - the number of images	
- _bike_parking_ - whether there's a bike parking near the building
- _is_studio_ - whether it's a studio	
- _is_open_plan_ - 	whether the plan is open
- _locality_name_ - the name of the locality	
- _airport_dist_ - the distance to the nearest airport	
- _city_center_dist_ - the distance to city center	
- _park_dist_ - the distance to park	
-_parks_within_3000_ - the number of parks within 3000 meters	
- _pond_dist_ - the distance to pond	
- _ponds_within_3000_ - the number of ponds within 3000 meters
