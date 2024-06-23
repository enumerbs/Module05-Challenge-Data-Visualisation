# Module05-Challenge-Data-Visualisation
Data Analytics Boot Camp - Module 05 - Data Visualisation \
Matplotlib Challenge

---

# Results

TBA:
- path1
- path2

# Implementation notes

TBA

# References

The following references were used in the development of the solution for this Challenge.

## Matplotlib - pie chart - 'title' positioning; wedge 'color' control
- https://www.pythoncharts.com/matplotlib/pie-chart-matplotlib/

NOTE: 'title' positioning seems to be limited to left/centre/right horziontally, but that by accessing the Figure's Axes object(s) we can use Axes.set_ylabel() to create a vertically centred 'title' on the 'y axis':
- https://stackoverflow.com/questions/21191519/python-matplotlib-moving-graph-title-to-the-y-axis

Default colour scheme colours can be accessed via the 'default property cycle':
- https://matplotlib.org/stable/gallery/color/color_cycle_default.html 
## Pandas - group by / filtering using value_counts()
- https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.value_counts.html
- https://stackoverflow.com/questions/64234573/how-to-find-the-length-of-value-counts-that-is-greater-than-1-in-a-pandas-data

## Pandas - returning unique values from one part of a MultiIndex
Inspired by Scott Boston's response post on the following page:
- https://stackoverflow.com/questions/53286882/how-to-reindex-a-multiindex-dataframe