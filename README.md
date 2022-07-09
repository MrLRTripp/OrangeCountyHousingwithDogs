# OrangeCountyHousingwithDogs

## Exploratory Data Analysis of Orange County, California Pet License data set combined with US Census Housing Survey.

**Purpose:** Try to determine if there is any correlation between dog ownership and housing data. Compare Orange County results with Seattle, WA results.

The Orange County, California dog license data was provided as part of a data request I made. (See 22-3152.pdf) It has about 7700 rows of data on dogs mostly from May and June 2022. A full 12 months would give a more accurate picture of the dogs that are registered in each zip code, but two months seems sufficient to compute the correlations with housing data from the Census.

The data was provided as a text-based pdf file. Luckily, the Camelot package for python can extract the data.
https://camelot-py.readthedocs.io/en/master/

Census data can be found at:

https://data.census.gov/cedsci/table?t=Housing%3AHousing%20Units%3AOccupancy%20Characteristics%3AOwner%2FRenter%20%28Householder%29%20Characteristics%3AOwner%2FRenter%20%28Tenure%29&g=0400000US06_0500000US06059,06059%248600000&y=2020&tid=ACSDP5Y2020.DP04

The downloaded CSV file is: ACSDP5Y2020.DP04_data_with_overlays_2022-07-06T151600.csv

## Conclusion

Similar to what we saw with the Seattle data (https://github.com/MrLRTripp/SeattleHousingwithPets), dog ownership is highly correlated with a zip code's owner occupancy percentage as well as to the zip code's percentage of 4 and 5 bedroom homes. Not surprisingly, owner occupancy percentage is highly correlated with percentage of 4 and 5 bedroom homes.

Unlike the Seattle data, we do see a moderate correlation with property value and rent. Again, because these are moderately correlated with 4 and 5 bedroom homes.

Strong *negative* correlation with areas that have no bedrooms or 1 or 2 bedrooms.

**Bottom line:** households with bigger homes with higher value are most likely to own a dog.
