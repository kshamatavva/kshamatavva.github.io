---
name: In Class Example
tools: [Python, HTML, vega-lite]
image: assets/from_vega_editor.png
description: In Class Example
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# In Class Walkthrough

Getting some practice saving ALtair/bega-lite json schemas for our Jekull page.

## Case 1: Saving from vega- lite editor

This I created by going to the [vega-editor](https://vega.github.io/editor) and making sure I used the [vega-datasets](https://raw.githubusercontent.com/vega/vega-datasets/refs/heads/master/data/barley.json) direct link to the data and saving with the "Export" from the vega editor.

<vegachart schema-url="{{ site.baseurl }}/assets/json/from_vega_editor.json" style="width: 100%"></vegachart>

## Case 2: Saving from Altair

Now we'll learn how to save our specficatiosn for inclusion from a python notebook.

### Sub-case 2a: With remotely hosted data

<vegachart schema-url="{{ site.baseurl }}/assets/json/saved_plot1_sp24.json" style="width: 100%"></vegachart>

### Sub-case 2b : With data saved from Python

<vegachart schema-url="{{ site.baseurl }}/assets/json/saved_plot2_sp25.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/mobility.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/kshamatavva/kshamatavva.github.io/blob/main/python_notebooks/inClass_week11.ipynb" text="The Analysis" %}
</div>

