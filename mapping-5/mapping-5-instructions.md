# Geography 109:<br>Digital Mapping<br>Mapping 5: Missing Data

University of Kentucky
<br>Matthew W. Wilson

In this exercise, you will work with a data set of unknown origin where values maybe be missing and you as a GIS specialist have to explain why the data is missing, how to address this issue, and what the implications for missing or misused data may be. Use QGIS and US Census data to explore this issue in fuller detail through the exercise.

**Note** You may need a review on how to manipulate data and render it in QGIS. Refer to [Mapping 4](../mapping-4/README.md) for additional details.

## Instructions

1. Your associate has handed you a file on occupancy in Fayette County, KY. There was no information on how old this data is, but they stated that the person they received it from said it was recent information. They have tasked you with mapping areas of high vacancy in Fayette county. Open [the file](assets/fayette_block_occupancy.csv) in Excel (or spreadsheet program of your choice) and exam the data.

2. We notice that the data contains numbers of total, occupied, and vacant households in the Fayette County area at the block level. Now that we know our data set contains vacancy information, we need to find a spatial data set to join our data to. Open QGIS and load a recent data set from the US Census Bureau for [2010 Fayette County Blocks](assets/tl_2010_21067_tabblock10.zip).

3. Unzip the above file and load the shapefile it into QGIS.

  ![Image31](assets/images/31.jpg)

4. We now need to load the occupancy data into QGIS and join it to our shapefile. We can make the join using **Id2** in the occupancy data set to the **GEOID10** column in our shapefile.

5. Next, we want to 

## Questions

1. In reviewing the occupancy data, what does the value of zero mean? Is this different than having no value at all? Explain your answer.

