# Crop-Yields
## Final Capstone for the 30-Day Challenge by [Zindua School](https://zinduaschool.com)

This project involves: database design, data consolidation into an relational databse, as well as data analysis and visualisation on global crop yields. 

# Global Crop Yields

The data this week comes from [Our World in Data](https://ourworldindata.org/crop-yields). Note that there is a lot of data on that site, we're looking at some subsets but feel free to use whatever data from there you find interesting! It's all pretty clean and ready to go.

Also note that there are cases where the long data includes both continent (eg Africa, Americas), countries (USA, Afghanistan, etc) and regions (North Asia, East Asia, etc). You'll need to be careful making assumptions when grouping and/or excluding specific groups.

> Our data on agricultural yields across crop types and by country are much more extensive from 1960 onwards. The UN Food and Agricultural Organization (FAO) publish yield estimates across a range of crop commodities by country over this period. The FAO report yield values as the national average for any given year; this is calculated by diving total crop output (in kilograms or tonnes) by the area of land used to grow a given crop (in hectares). There are likely to be certain regional and seasonal differences in yield within a given country, however, reported average yields still provide a useful indication of changes in productivity over time and geographical region.

We've also included data on the trade off between higher yields and land use, so there are some interesting changes to track beyond raw production.


### Data Dictionary

# `key_crop_yields.csv`

|variable                         |class     |description |
|:--------------------------------|:---------|:-----------|
|Entity                           |character | Country or Region Name |
|Code                             |character | Country Code (note is NA for regions/continents) |
|Year                             |double    | Year |
|Wheat (tonnes per hectare)       |double    | Wheat yield |
|Rice (tonnes per hectare)        |double    | Rice Yield |
|Maize (tonnes per hectare)       |double    | Maize yield |
|Soybeans (tonnes per hectare)    |double    | Soybeans yield |
|Potatoes (tonnes per hectare)    |double    | Potato yield |
|Beans (tonnes per hectare)       |double    | Beans yield|
|Peas (tonnes per hectare)        |double    | Peas yield |
|Cassava (tonnes per hectare)     |double    | Cassava (yuca) yield|
|Barley (tonnes per hectare)      |double    | Barley|
|Cocoa beans (tonnes per hectare) |double    | Cocoa |
|Bananas (tonnes per hectare)     |double    | Bananas |

# `arable_land`

|variable                                                               |class     |description |
|:----------------------------------------------------------------------|:---------|:-----------|
|Entity                           |character | Country or Region Name |
|Code                             |character | Country Code (note is NA for regions/continents) |
|Year                             |double    | Year |
|Arable land needed to produce a fixed quantity of crops ((1.0 = 1961)) |double    | Arable land normalized to 1961 |


# `fertilizer`

|variable                                        |class     |description |
|:-----------------------------------------------|:---------|:-----------|
|Entity                           |character | Country or Region Name |
|Code                             |character | Country Code (note is NA for regions/continents) |
|Year                             |double    | Year |
|Cereal yield (tonnes per hectare)               |double    | Cereal yield in tonnes per hectare |
|Nitrogen fertilizer use (kilograms per hectare) |double    | Nitrogen fertilizer use kg per hectare |

# `land_use`

|variable                                                  |class     |description |
|:---------------------------------------------------------|:---------|:-----------|
|Entity                           |character | Country or Region Name |
|Code                             |character | Country Code (note is NA for regions/continents) |
|Year                             |double    | Year |
|cereal yield index                                        |double    | Cereal yield index |
|change to land area used for cereal production since 1961 |double    | Change to land area use for cereal production relative since 1961|
|total population (gapminder)                              |double    | Total population from gapminder data |

# `tractor`

|variable                                              |class     |description |
|:---------------------------------------------------------|:---------|:-----------|
|Entity                           |character | Country or Region Name |
|Code                             |character | Country Code (note is NA for regions/continents) |
|Year                             |double    | Year |
|Tractors per 100 sq km arable land                    |double    | Number of tractors per 100 sq km of arable land |
|Cereal yield (kilograms per hectare) (kg per hectare) |double    | Cereal yield in kg per hectare |
|Total population (Gapminder)                          |double    | Total population from gapminder |

## Deliverables 
The following are the outcomes expected from the project: 
1. Create a logical and physical SQL Schema - Have it separate and upload it to your GitHub repo
2. Create the the Databases and the tables to contain the data - millitary, age, year - Have it separate and upload it to your GitHub repo
3. Load the data to Power BI and Perform transformations - e.g cleaning the age column, formatting datatypes 
4. Develop Power BI Visualizations 
5. Develop a Power BI - Dashboard 
6. Presentation with Insights.

### Project Collaborators
- **Agnes Mutembei:** Enter short bio | [Github]() | [LinkedIn]()
- **Zainab Chepkosgei:** Enter short bio | [Github]() | [LinkedIn]()
- **Shirley Odak:** Enter short bio | [Github]() | [LinkedIn]()




