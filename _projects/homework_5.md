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

In theory, you can also use [Jekyll hooks](https://jekyllrb.com/docs/plugins/hooks/) to do it, but I haven't figured out a way that looks nice yet.

<vegachart schema-url="{{ site.baseurl }}/assets/json/saved_plot5_sp25.json" style="width: 100%"></vegachart>



## Search The Data & Methods



<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

