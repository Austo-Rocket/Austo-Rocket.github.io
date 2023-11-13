---
name: Building Inventory Dataset 
tools: [Python, HTML, vega-lite]
image: assets/pngs/visualization(1).png
description: This is a "showcase" for my IS-445 course that uses vega-lite and Altair to solve HW 8
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Building Inventory Dataset



### Visualization 1: How total floors of buildings change over time



<vegachart schema-url="{{ site.baseurl }}/assets/json/chart1.json" style="width: 100%"></vegachart>

###### This code displays a scatter plot using Altair, representing data from a building inventory. Each point in the scatter plot corresponds to a building and is positioned based on the year it was constructed (on the x-axis) and the total number of floors it has (on the y-axis). The color of each point represents the total number of floors as well light blue being low floors dark blue being high floors. The data can be filtered by county using a dropdown menu, and a brush selection allows for filtering based on a specific range of years and total floors. This plot could help understand how buildings have changed throughout time including floors and square footage. In the data we can see an increase of floors in more recent years. I put a dropdown menu to provide a choice for selecting a specific county. The chart is then filtered to display only the buildings from the selected county. This allows users to focus on specific regions and compare the distribution of buildings across different counties. The brush selection enables users to interactively choose a specific range of years and total floors. This can be useful for analyzing patterns or trends within a particular time period or range of total floors.

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


