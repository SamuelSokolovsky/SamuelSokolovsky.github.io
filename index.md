---
layout: default
title: HW5
---

# HW5: Two Visualizations of License Data

[The Data](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/licenses_fall2022.csv)

[The Analysis]([(https://github.com/SamuelSokolovsky/SamuelSokolovsky.github.io/blob/main/is445_hw5.ipynb)])

## Visualization 1

PASTE YOUR FIRST CHART IMAGE OR EMBED HERE

The first visualization shows the distribution of license types in the dataset by counting how many entries fall into each category. A bar chart was used because it clearly displays categorical comparisons. The x-axis represents the license type, while the y-axis shows the count of each type. Color was also mapped to license type to make the categories easier to distinguish visually. On the data side, the dataset was loaded from a URL and no major transformations were required beyond counting occurrences of each category. This design choice allows for a straightforward comparison of which license types are most common.

## Visualization 2

PASTE YOUR SECOND CHART IMAGE OR EMBED HERE

The second visualization also explores license types but introduces interactivity to enhance the analysis. Similar encodings were used, with license type on the x-axis and count on the y-axis, but this chart includes a selection feature that allows users to click on a category to highlight it while dimming the others. This was implemented using an Altair selection, which improves clarity by helping users focus on one category at a time without losing context. The interactivity makes the chart more engaging and useful for exploring patterns in the data. As with the first chart, the data was read directly from the source URL and processed using basic aggregation.
