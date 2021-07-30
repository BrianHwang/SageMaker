# corr()

https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.corr.html

DataFrame.corr(method='pearson', min_periods=1)

* Method of correlation
- pearson : standard correlation coefficient : https://en.wikipedia.org/wiki/Pearson_correlation_coefficient
- kendall : Kendall Tau correlation coefficient : https://en.wikipedia.org/wiki/Kendall_rank_correlation_coefficient
- spearman : Spearman rank correlation : https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient

correlation coeffiecnt only measure **linear** correlation.
correlation coeffiecnt range from -1 to 1.
1 : string positive correation : mediaium house value up, medium income value up.
-1 : string negative correction : 
0 : no linear correation.


TODO : book page 58

example with heatmap
```
corr_matrix = salary_df.corr()
sns.heatmap(corr_matrix, annot=true)
plt.show()
```

book example
```
corr_matrix = houseing.corr()

corr_matric["median_house_value"].sort_values(ascending=False)
```

# scatter_matrix()
https://pandas.pydata.org/docs/reference/api/pandas.plotting.scatter_matrix.html
https://seaborn.pydata.org/examples/scatterplot_matrix.html

plots every nermuric attributes against other numeric attributes.
```
from pandas.plotting import scatter_matrix

attributes = [.....]
scatter_matrix(housing[attributes], figsize(12,8))

#zoom in
housing.plot(kind="scatter", x="median_income", y="dedian_house_value", alpha=0.1)
```
