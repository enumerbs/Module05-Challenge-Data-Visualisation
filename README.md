# Module05-Challenge-Data-Visualisation
Data Analytics Boot Camp - Module 05 - Data Visualisation \
Matplotlib Challenge

---

# Results

Refer to the Jupyter Notebook, file: Pymaceuticals/pymaceuticals.ipynb.

# Implementation notes

## Data cleansing

Where a 'Mouse ID' and its corresponding tumour size measurement 'Timepoint' were repeated, such cases were removed from consideration for the remaining analysis (as otherwise the measurement result would be ambiguous).
- A Pandas-based approach using grouping via the 'value_counts()' method was used to identify such cases (value counts greater than one indicating 'duplicates').
- The 'Mouse ID' for any 'duplicate mouse' measurement could then be extracted from the grouping.
- Refer to the Pandas references below for more information on both those implementation details.

## Summary Statistics

Statistics calculated for the tumor size measurement include:
- Mean
- Median
- Variance
- Standard Deviation
- Standard Error of the Mean (SEM)

## Data Visualisation

Charts and plots used to describe the data and results analysis include:
- Bar charts
- Pie charts
- Boxplots
- Line charts
- Scatter plots (including overlay of linear line).


# References

The following references were used in the development of the solution for this Challenge.

## Pandas - group by / filtering using value_counts()
- https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.value_counts.html
- https://stackoverflow.com/questions/64234573/how-to-find-the-length-of-value-counts-that-is-greater-than-1-in-a-pandas-data

## Pandas - returning unique values from one part of a MultiIndex
Inspired by Scott Boston's response post on the following page:
- https://stackoverflow.com/questions/53286882/how-to-reindex-a-multiindex-dataframe

## Matplotlib - pie chart - 'title' positioning; wedge 'color' control
- https://www.pythoncharts.com/matplotlib/pie-chart-matplotlib/

NOTE: 'title' positioning seems to be limited to left/centre/right horziontally, but that by accessing the Figure's Axes object(s) we can use Axes.set_ylabel() to create a vertically centred 'title' on the 'y axis':
- https://stackoverflow.com/questions/21191519/python-matplotlib-moving-graph-title-to-the-y-axis

Default colour scheme colours can be accessed via the 'default property cycle':
- https://matplotlib.org/stable/gallery/color/color_cycle_default.html

## Matplotlib - box plots - median line colour, outlier colour & other formatting options
- https://nrecursions.blogspot.com/2021/02/changing-colors-in-pandas-boxplot.html
- https://stackoverflow.com/questions/43342564/flier-colors-in-boxplot-with-matplotlib
