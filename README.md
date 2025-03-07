# Northern Red Oak Climate Change Analysis

Evaluating the effects of climate change and fire occurance on northern red oak habitat range.

## Project Contents

- [Data Source](#data-source)
- [Project Background](#project-background)
- [Purpose](#purpose)
- [Mapmaking Process](#mapmaking-process)
- [Map Summary](#map-summary)
- [Final Project Link](#final-project-link)

***

### Data Source

1. Eastern United States Climate Change Tree Atlas – Suitable Habitat for *Quercus rubra* (Northern Red Oak) as Measured by Importance Value (IV)
[Link to data source](https://databasin.org/datasets/bc998e667164491090052196ceaf12ae/)
2. USTreeAtlas: Clone of Digital Representations of Tree Species Range Maps from "Atlas of United States Trees" by Elbert L. Little, Jr. (and other publications)
[Link to data source](https://github.com/wpetry/USTreeAtlas/tree/main)
3. Spatial wildfire occurrence data for the United States, 1992-2020
[Link to data source](https://www.fs.usda.gov/rds/archive/catalog/RDS-2013-0009.6)

* Initial Data projection: WGS 84 (EPSG:4326)
* Final Map projection:WGS 84 (EPSG:4326)

### Project Background

If you are interested in [other Markdown formatting options](https://www.markdownguide.org/basic-syntax/)

### Purpose

Northern red oak (*Quercus rubra*) like many other tree species, will most definitely be negatively affected by current and future climate change. One concern is if current species’ ranges will continue to be suitable habitat in the future. The purpose of these maps is to analyze the effects of climate change and fire pressure on northern red oak range shifts. 

### Mapmaking Process

Example of in process map ![in process image](filepath)

You can describe the mapmapking process in this section, including images where it helps to describe the process.

You can also use some lists, and here's some formatting ideas.

1. First step in the mapmaking process was to find suitable data sets. I conducted a google search for data sets (shape files and geojson files) relating to northern red oak.
2. I loaded those files into QGIS where I further manipulated the data. I had 3 data files that included northern red oak range, fire occurrence data from 1992-2020, and modeling data on future northern red oak range with climate change.
3. For the northern red oak range data, I adjusted the color and opacity of the layer to make it more visually appealing.
4. For the modeled data I filtered the data in the attribute table to just include the Geophysical Fluid Dynamics Laboratory model data for RCP 4.5. I then created a duplicate layer and filtered the data for the Geophysical Fluid Dynamics Laboratory model data for RCP 8.5. I then overlayed the current northern red oak range layer on both maps for comparison. 
5. I used the Clip processing tool in QGIS to select only the fire data within the current northern red oak range, future northern red oak range at low (RCP 4.5) emissions, and future northern red oak range at high (RCP 8.5) emissions.
6. After selecting the fire range data accordingly, I used the Heatmap processing tool in QGIS to take the fire point data and project it as the number of fires within the oak range. This allows for a better identification of hotspots of reoccurring fire incidences.
7. I then exported 6 separate maps for different data visualization. 


### Map Summary

What are the key findings to take from your map and the overall mapmaking process?

## Final Project Link

Here you are linking from the README.md to the index.html.

Please view the [final map online](www.github...)