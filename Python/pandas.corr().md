https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.corr.html

DataFrame.corr(method='pearson', min_periods=1)

* Method of correlation
- pearson : standard correlation coefficient : https://en.wikipedia.org/wiki/Pearson_correlation_coefficient
- kendall : Kendall Tau correlation coefficient : https://en.wikipedia.org/wiki/Kendall_rank_correlation_coefficient
- spearman : Spearman rank correlation : https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient

TODO : book page 58

example with heatmap
```
corr_matrix = salary_df.corr()
sns.heatmap(corr_matrix, annot=true)
plt.show()
```
