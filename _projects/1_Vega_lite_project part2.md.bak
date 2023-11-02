---
name: Week 8 Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a week 8 home assignment.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Example 1 including vega-lite

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).
The distribution of buildings among the various congressional districts is seen in this bar chart. 
Buildings are classified along the x-axis by 'Congress Dist', which is a nominal variable (N), 
And the y-axis measures the 'count()' of buildings in each district. 
There is an instant visual difference between the districts because 
Each bar is colored in accordance with its corresponding congressional district. 
By using a color-coded categorical variable, the data for each district can 
Be easily distinguished visually, which facilitates straightforward comparisons.

This visualization uses the data directly to count the number of buildings in each congressional 
District; no significant data changes are made. 
This chart is a simple static depiction of the spread of buildings; 
It lacks any interactive elements. The chart's clarity is ensured by its simplicity, 
Which makes it easy to see which districts have more or less structures. 
However, to enable a more in-depth analysis of the data, interactivity might be included in a 
Manner similar to that of the preceding chart.



```
<vegachart schema-url="{{ site.baseurl }}/assets/json/cars.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization1.json" style="width: 100%"></vegachart>

In theory, you can also use [Jekyll hooks](https://jekyllrb.com/docs/plugins/hooks/) to do it, but I haven't figured out a way that looks nice yet.


## Example 2

<vegachart schema-url="{{ site.baseurl }}/assets/json/visualization2.json" style="width: 100%"></vegachart>

Below is where we can put some links to both the data and the analysis code as buttons:
We can use a vegachart HTML tag like so: The distribution of buildings by year of acquisition is 
Shown in this interactive histogram. The vertical axis, denoted as 'Year Acquired', 
Is a quantitative bin that shows the range of years that buildings were added to the inventory. 
The number of buildings that fall into each year bin is shown on the y-axis. By binning the 
'Year Acquired' variable, the design decision streamlines the data into more digestible periods, 
Highlighting trends in building acquisitions over time. A user-selectable interactive slider 
Augments the usefulness of the chart by permitting an interactive examination of the dataset.
 Altair's alt.binding_range slider and alt.selection_point selection mechanism, which filter
 data based on user input, provide interactivity.
 
 There is not much data transformation involved; Altair's binning and counting features are 
 Mostly used to arrange the data in a way that makes sense for the histogram. The interactive
 Filter that is applied to the dataset is the main transformation. It reacts to user input 
 Through the slider and dynamically updates the histogram to show the range of years that 
 Have been chosen. Because it enables users to identify specific interest periods within 
 The dataset, this interactive feature is both entertaining and educational. It improves 
 The clarity of the visualization and customizes it to the interests of the user.

```
<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

