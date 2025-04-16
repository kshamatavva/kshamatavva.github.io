---
name: Homework Number Five
tools: [Python, HTML, vega-lite]
image: assets/pngs/visualization.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Chart 1

<vegachart schema-url="{{ site.baseurl }}/assets/json/saved_plot4_sp25.json" style="width: 100%"></vegachart>

## Write Up 1

This visualization shows the total square footage of buildings managed by each agency, based  on the year the building was constructed and acquired. For this design, I used a vertical bar chart with nominal encoding on the x-axis (Agency Name) and quantitative encoding on the y-axis (Square Footage). I filtered the dataset to include only rows where Year Type equals "Year Constructed" after melting some features to combine the acquisition and construction years into a single column. Rows with missing square footage or year data were removed to maintain accuracy. While no color scheme is used in this version, the simplicity helps keep the focus on the square footage between agencies. Interactivity could be added through tooltips or filtering, but this version emphasizes overall distribution patterns.

# Chart 2 With Interactivity

<vegachart schema-url="{{ site.baseurl }}/assets/json/saved_plot6_sp25.json" style="width: 100%"></vegachart>

## Write Up 2

This visualization shows the number of buildings by usage type across counties. Each dot indicates a usage category within a county; the vertical axis displays building counts, while the horizontal axis represents the counties. The chart illustrates the distribution of building types and allows users to filter by usage type for focused analysis. It utilizes a scatter plot with nominal encoding on the x-axis (County) and quantitative encoding on the y-axis (Count). Points are colored based on the selected usage type using a paired color scheme for clarity. Selecting a usage type dims other categories in gray, highlighting the chosen category for the user to identify specific counties for specific usage. This interactivity is facilitated by a dropdown menu created with alt.binding_select(), linking it to the Usage Description column. Additionally, data is aggregated via groupby() to count buildings by county and usage description. This feature allows engagement and comparison, allowing users to focus on specific usage types and identify specific trends.

## Search The Data & Methods



<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/kshamatavva/kshamatavva.github.io/blob/main/python_notebooks/homework_5.ipynb" text="The Analysis" %}
</div>

