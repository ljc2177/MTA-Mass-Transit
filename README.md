# MTA-Mass-Transit

These scripts create usable GIS layers in a shapefile format from the NYC MTA's static developer feeds. The GTFS route and timetable data from the feeds is generalized and simplified to create lines representing singular routes and points representing individual stops. 

Data output from the scripts can be regarded as being in a near-final state. The output should always be scrutinized, as manual corrections may be necessary due to: updates to the feed that necessitate changes in the script, data quality issues that appear in one iteration of the feed but disappear in the next, and a lag between what's represented in the data and reality. For example, as of Sept 2018 the static feeds still don't include the 2nd Avenue subway extension as a route, although it does include the stations as stops.

These scripts were originally written to create the [NYC Mass Transit Layers series](https://www.baruch.cuny.edu/confluence/display/geoportal/NYC+Mass+Transit+Spatial+Layers) produced by the GIS Lab at Baruch College CUNY. 

# Required libraries:
* urllib
* BeautifulSoup
* requests
* pandas
* geopandas
* shapely

# How to run
1. Clone the repo
2. open and run eiter main.py or main.ipynb to download the data and create shapefiels
