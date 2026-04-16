---
layout: default
title: HW5
---

# HW5: Two Visualizations of License Data

[The Data](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/licenses_fall2022.csv)

[The Analysis](https://github.com/SamuelSokolovsky/SamuelSokolovsky.github.io/blob/main/is445_hw5.ipynb)

## Visualization 1

<iframe src="{{ '/chart1.html' | relative_url }}" width="100%" height="600" style="border:none;"></iframe>

This visualization shows the number of Illinois professional licenses issued per year, broken down by license status. A line chart was used to display trends over time, with the x-axis representing the year of original issue and the y-axis showing the number of licenses issued. Color is used to see between different license statuses, allowing for easy comparison across categories. One pattern that is seen is that “NOT RENEWED” licenses consistently have the highest counts across most years, with a particularly large spike in the late 1990s, suggesting a significant increase in licenses that were not maintained during that period. In contrast, categories like “ACTIVE” and “INACTIVE” remain relatively stable with slow changes over time, while other statuses such as “CANCELLED” or “TERMINATED CARD RETURNED” appear less frequently. Overall, the visualization highlights long-term trends and differences in license outcomes across decades.

## Visualization 2

<iframe src="{{ '/chart2.html' | relative_url }}" width="100%" height="600" style="border:none;"></iframe>

This visualization shows the top 15 most common professional license types in Illinois based on the total number of licenses issued. A horizontal bar chart was used because it makes it easier to compare categories with long names and clearly rank them from highest to lowest. The y-axis represents the license type, while the x-axis shows the total number of licenses. Color is used to differentiate the bars, but mainly serves to improve how the chart looks rather than encode an additional variable. The data was transformed by grouping the dataset by license type and counting the number of occurrences, then selecting the top 15 categories to focus on the most relevant results. The chart reveals that “DETECTIVE BOARD” and “COSMO” licenses are by far the most common, having much more than all other categories, while the other license types have much smaller counts. This highlights how a few professions at the top of the dataset compared to others.
