---
name: Vega Lite Homework 6.1 (Plot 1) Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/static.png
description: This is a Homework 6 project that uses vega-lite for static viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Example including vega-lite

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).

We can use a vegachart HTML tag like so:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/static.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/static.json" style="width: 100%"></vegachart>


Plot 1: Degree Distribution Plot (Static Plot)
This bar chart visualizes the distribution of license counts among the users, focusing only on licensed users with more than one license. The x-axis is used to represent the binned numerical values of license counts, categorized into uniform intervals or bins for simplifying the graph in order to show patterns existing in data. The y-axis is used to represent the count of users falling into each bin, thus showing license distribution across individuals. A limited color scheme of steel blue was chosen to retain clarity without distraction. The data was transformed by grouping the records on user names and calculating the total number of licenses held by each user, then filtering out those users who hold only one license; this will ensure that analysis produces nonspurious trends in the data.



## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/sanyamiii/sanyamiii.github.io/blob/main/python_notebooks/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/sanyamiii/sanyamiii.github.io/blob/main/python_notebooks/Hw6.ipynb" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/sanyamiii/sanyamiii.github.io/blob/main/python_notebooks/licenses_fall.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/sanyamiii/sanyamiii.github.io/blob/main/python_notebooks/Hw6.ipynb" text="The Analysis" %}
</div>

