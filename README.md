# properties-data-wrangling
## Description
The notebook does 2 major tasks: Data Integration and Data Reshaping.  

The objective of the data integration task is to integrate 7 different data files in various formats such as xml, json, html, xlsx, gtfs and shapefiles. The data files are about house properties; the 2 real estate files contain information about the properties such as number of bedrooms, bathroom, year of property, price of the property, geocoordinates of the property. The shopping centres, supermarkets  and hospitals files have the list of shopping centres, supermarkets and hospitals respectively with their geocoordinates. The nearest utility to the property is found using these files and integrated in the consolided database of properties. The "VIC Boundary" shapefile has the boundaries of the suburbs in Melbourne. It is used to find the suburb of the properties. The GTFS file has information about Melbourne trains, and is used to find the nearest station to the property and the travel time to CBD.  

The objective of the data reshaping task is to perform various normalisation and transformations to the property price. These transformations are compared against each other. Finally, the transformations are contrasted against each other to fit a linear model for property price using the appropriate predictors. The best transformation for property price is finally recommended for a linear model.  

## Packages required
* pandas
* numpy 
* matplotlib
* scikit-learn
* statsmodels
* beautifulsoup4
* pyshp
* shapely
