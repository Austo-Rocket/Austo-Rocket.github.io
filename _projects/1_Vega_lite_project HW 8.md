---
name: Building Inventory Dataset 
tools: [Python, HTML, vega-lite]
image: assets/pngs/Viz(1).png
description: This is a project that shows the correlation of amount of crime, time of crime, and type of crime from 2011 to now
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Rockford Crime Dataset



### Visualization 1: What time crimes happen and their type in Rockford, Illinois from 2011 to now



<vegachart schema-url="{{ site.baseurl }}/assets/json/RockfordViz.json" style="width: 100%"></vegachart>


### Dataset Information


######  The name of the dataset is "City of Rockford Crime Offenses 2011-Present." I obtained this dataset from the data.illinois.gov website that is posted in the FP1.1. The data set can be found at this URL: "https://data.illinois.gov/dataset/116city_of_rockford_crime_offenses_2011present." While there was no explicit stating of license, in the about the dataset it says that the data is obtained form the NETRMS records management system and that the data should not be used comparative reporting. In the about data.illinois.gov section it says that "Illinous Open Data Portal lets you find data across state, find facts about your state, lets you create maps and graphs, and lets you freely download the data for your own analysis." The file is 22MB large, but github has up to 2 GB max file size for free. Seeing that the file is under the maximum file size I should be find hosting the data myself. 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/Austo-Rocket/Austo-Rocket.github.io/blob/822d693237d745d4a1821318cb4d8b3c16cbcada/python_notebooks/WorkbookHW8.ipynb" text="The Analysis" %}
</div>


### Visualization 2: Building usage description and Congressional Full Name

<vegachart schema-url="{{ site.baseurl }}/assets/json/chart_usage.json" style="width: 100%"></vegachart>

###### For this chart I had to first limit the amount of rows that displayed as there was a 5000 maximum. The y-axis represents the "Usage Description" of buildings, and the x-axis represents the "Congressional Full Name" of the buildings. This is to better understand which people own buildings for which purposes. The interactivity in the plot is added so you can hover over a spot and see the specific Name and Usage.


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Austo-Rocket/Austo-Rocket.github.io/blob/822d693237d745d4a1821318cb4d8b3c16cbcada/python_notebooks/WorkbookHW8.ipynb" text="The Analysis" %}
</div>


