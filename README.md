# Analysis of Business Ventures in Kolkata

```
Searching for place in kolkata city, capital of West Bengal to launch pizza place, indian restaurant and hotel
```
```
Swattik Chakrabarty
```
**Introduction:**

Kolkata is considered one of the largest cities in India. It is among the
top metro cities in India and is the capital of West Bengal.
Nowadays, the hotel management industry is becomingone of the
leading industries among all. This project deals withthe major venue
categories in the neighborhoods of Kolkata. This projectwould
specifically help Business personnels plan, to startnew restaurants,
hotels, pizza places, etc.

#### Aim:

This project aims to find the best location to opena pizza place,Indian
restaurant and hotel in the city of joy, Kolkata,to maximize the profit of
the owner. We want to open these in a neighborhoodwhich are
attractive in business aspects yet less crowded withalready existing
venues as mentioned above.

## Data Requirements:


★Dataset containing Neighborhoods of Kolkata- Thisdataset holds
the names of Neighborhoods and Landmarks in Kolkataextracted
from Nivalink with the help of Beautiful Soup package.



○ Here is a link to the dataset
http://www.nivalink.com/localities-and-landmarks/kolkata

★Python library geopy was used to get the coordinatesof
neighborhoods in the dataset. Data required repeatedcalls from
geopy to correctly give the coordinates of Neighborhoodsof
Kolkata in the used data frame.

★Foursquare API was used to extract the most commonplaces of a
neighborhood in the form of a JSON file and was putin the final
dataset to explore the venues.

### Methodology:

As our data does not have the coordinates of the location that we extracted,
we will use the geocoder package to get the latitudes and longitudes of 65
neighborhoods. With the help of Folium let's visualizethe neighborhood
data that we collected. This will be done by using the coordinates of the
location that we collected and updated in our pandas dataset.Here with the
help of the FourSquare API we will try to collect popular venues around
our locations. In order to make a good prediction and create a good
analysis let's consider only the neighborhoods with more than 40 venues,
as the neighborhoods with less than 40 venues are less popular and hence
less populated. So as we want the new business owner to make profit in
their ventures we should only consider neighborhoods which are
popular.

We performed one hot encoding on the obtained data set and used
it to find the 10 most common venue categories ineach neighborhood.
Then clustering can be performed on the dataset.Weare using the K -
Nearest Neighbor clustering technique. To find theoptimal number of
clusters, silhouette score technique is used. Initially,in the original data
frame we only had the neighborhoods with their top10 venues. After
fitting the data on the K-means model we insert anew column in the
pandas dataframe, as cluster label, with the helpof our model so that each
neighborhood can be identified with the name of theircluster and
segregation of neighborhoods according to their respectivecluster can take
place

![Imgur](https://imgur.com/1kT3oZl.png)


### Results:


![Cluster1](https://imgur.com/dgo8sOD.png)
● There are 15 Pizza places ,15 Multiplex , 14 IndianRestaurant and 8 Hotels in
cluster 1

![Cluster2](https://imgur.com/NjXhms7.png)
● As there are no pizza places in the top 10 venuesof this cluster hence the
number of pizza places must be less than 10 becausehere the 10th most
popular venue is a pub whose value count is 10. Thereare 18 Multiplex , 30
Indian Restaurant and 30 Hotels in cluster 2

![Cluster3](https://imgur.com/sqH5SPX.png)
● As there are no Multiplexes and Hotels in top 10 venuesof this
cluster hence the number of multiplexes and Hotelsmust be less
than 3 because here the 10th most popular venue islounge whose
value count is 3.There are 5 Pizza Places and 5 IndianRestaurant a
in cluster 3

![Cluster4](https://imgur.com/AXt1dHA.png)
● As there are no pizza places and Indian restaurants in top 10 venues
of this cluster hence the number of pizza places andIndian restaurant
must be less than 2 because here the 10th most popularvenue is
Bengali restaurant whose value count is 2. There are3 Multiplexes
and 3 Hotels in Cluster 4

![Graphs](https://imgur.com/OuFVLmE.png)

## Discussion/Observation:


## Hotels:

As there are no pizza places and Indian restaurantsin the top 10 venues of
this cluster hence the number of pizza places andIndian restaurants must
be less than 2 because here the 10th most popularvenue is Bengali
restaurant whose value count is 2. There are 3 Multiplexesand 3 Hotels in
Cluster 4

## Fast Food Restaurant:

Cluster 3 and Cluster 4 are the least popular withthe lowest number of neighborhoods
and venues hence opening a fast food restaurant herewill not fetch the owner profits
Out of the most popular clusters i.e, Cluster 1 andCluster 2, the neighborhoods in
cluster 1 has the greatest number of fast food restaurants(15),hence opening one here
is not ideal.


Thus opening a hotel in Cluster 2 is most ideal as it has multiple popular and most
neighborhood options and no fast food restaurants. This rarity of fast food restaurants
in such a popular cluster can be utilized by businessventurers to maximize profits.

Potential Neighborhoods are: Tollygunge Metro Station,EsplanadeMetro Station,Fort
William

## Pizza Place:

Cluster 1 has the most number of Pizza Places, soit doesn't make any sense to open a
Pizza Place there.

However Cluster 2 being the most popular and crowdedplace among all the clusters,
and if it does have any pizza place it will be lessthan 8. Hence the most popular place
to open a pizza place is Cluster 2. AlternativelyCluster 3 and Cluster 4 can also be
suggested as Cluster 3 has only 5 and Cluster 4 doesnot have any. But as cluster 4 is
the least popular it is probably not a good idea toopen it there.

Potential neighborhoods to open: Townhall, EsplanadeMetro Station, Fort William

## Multiplexes:

The most popular clusters are crowded with multiplexesso opening a multiplex there
will face a lot of competition.

Cluster 4 being the least lost popular cluster isstill crowded with multiplexes(5).
Hence Cluster 3 is the most suitable to open a multiplexas it is relatively popular than
Cluster 4 and even if it has multiplexes then theywill be less than 3 therefore it will
face less competition.

Potential neighborhoods to open: Tollygunge MetroStation, Kalighat


## Conclusion:

Reason for this venture was to investigate the neighborhoodsof Patna and make a
grouping model to recommend spots to begin anotherbusiness dependent on the class.
The neighborhoods information was gotten from nivalinkand the Foursquare API was
utilized to track down the significant settings inevery area. Then, at that point areas
were utilized to make a bunching model. The best numberof bunches for example 4
was acquired utilizing the outline score. Each bunchwas analyzed to track down the
most scene classes present, that characterizes thequalities for that specific group. A
guide showing the bunches has been given. Both ofthese can be utilized by partners to
choose the area for the necessary kind of business.


