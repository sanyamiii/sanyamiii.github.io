---
name: Vega Lite Homework 6 Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/visualization.png
description: This is a Homework 6 project that uses vega-lite for interactive viz!
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
<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization.json" style="width: 100%"></vegachart>

Plot 2: Interactive Scatter Plot of License Types (Binned)
This scatter plot investigates the number of licenses binned versus their original values, adding an extra layer of interactivity by license type. The x-axis has license numbers binned into 20 segments, while the y-axis is the original license numbers. Each point is colored by the license type, which helps in differentiating these different categories. Everything outside the chosen filter is grayed out so that the visualization shows only the interesting subset of data. Tooltips add more information, like license numbers and types, also an ID, which gives more insight to the exploration. Data Preparation: Correct errors in the License Number column by converting invalid values to NaN, dropping rows containing invalid values, and ensuring the column was of integer type. A sample of 500 rows was also taken so that the visualization is manageable to view. Binning has been applied to systematically group license numbers, making this a clearer and more accessible visualization.                                                     


Discussion of Interactivity
This is the interactive scatter plot that adds so much to its clarity and appeal. Filtering by specific license types is made enabled through the dropdown menu option, thus helping in focusing on certain categorical groups. The brush selection allows users to highlight specific regions in the data, which makes it easier to see certain trends or patterns that aren't readily apparent. The combination of interactivity added in here makes the visualization even more dynamic, showing users more effectively the deeper insights into the dataset's relationships.

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

