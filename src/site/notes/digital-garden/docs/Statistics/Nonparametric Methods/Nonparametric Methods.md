---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/nonparametric-methods/"}
---

Nonparametric statistics are a class of statistical methods used when _the data do not meet the assumptions of parametric statistics_. Parametric statistics typically assume that the data follow a specific probability distribution (usually the normal distribution) and that the parameters of this distribution are known or can be estimated from the data. Nonparametric statistics, on the other hand, **make fewer or no assumptions about the underlying distribution of the data** and are often used when dealing with categorical, ordinal, or skewed data.

![Pasted image 20231016053701.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016053701.png)

Here are some key aspects and methods of nonparametric statistics:

1. **Data Types**: Nonparametric methods are particularly useful when dealing with non-normally distributed data, [[digital-garden/docs/Statistics/Data Analysis and Visualization/Data Type/Ordinal Data\|Ordinal Data]] (data with ordered categories but unknown intervals between them), or [[digital-garden/docs/Statistics/Data Analysis and Visualization/Data Type/Nominal Data\|Nominal Data]] (categorical data with no inherent order). 

2. **[[Ranking\|Ranking]]**: Many nonparametric tests involve ranking the data, which transforms the original data into a more tractable form. This ranking is often based on the order of values, rather than their actual numerical values.

3. **[[digital-garden/docs/Statistics/Data Analysis and Visualization/Descriptive Statistics/Median\|Median]]**: Instead of using the mean (average), nonparametric statistics often rely on the median (middle value) to describe central tendency because it is less sensitive to extreme outliers.

4. **[[digital-garden/docs/Statistics/Inference/Hypothesis testing/Hypothesis testing\|Hypothesis testing]]**: Nonparametric tests are used for hypothesis testing, just like parametric tests. Some common nonparametric tests include:

   - **Mann-Whitney U Test ([[digital-garden/docs/Statistics/Inference/Hypothesis testing/The Wilcoxon Rank-Sum Test\|The Wilcoxon Rank-Sum Test]])**: Used to compare two independent groups or samples to determine if there is a statistically significant difference between them.
   
   - **Kruskal-Wallis Test**: An extension of the Mann-Whitney test, used for comparing three or more independent groups.

   - [[digital-garden/docs/Statistics/Inference/Hypothesis testing/The Wilcoxon Rank-Sum Test\|The Wilcoxon Rank-Sum Test]]: Used to compare two related samples or paired data to assess whether there is a statistically significant difference between them.

   - **[[Chi-Square Test\|Chi-Square Test]]**: Used for analyzing the association between categorical variables in a contingency table.

   - **Friedman Test**: An extension of the Wilcoxon signed-rank test used for comparing three or more related samples.

   - **Runs Test**: Used to test whether a sequence of data is random or exhibits some form of systematic pattern.

5. **Goodness-of-Fit Tests**: Nonparametric goodness-of-fit tests, such as the Kolmogorov-Smirnov test and the Anderson-Darling test, are used to assess whether a sample comes from a specific distribution.

6. **[[Correlation Analysis\|Correlation Analysis]]**: Nonparametric methods like the Spearman rank correlation coefficient are used to assess the strength and direction of associations between variables when the assumptions of parametric correlation (e.g., Pearson correlation) are not met.

7. **Resampling Methods**: Bootstrapping and permutation tests are nonparametric techniques that involve repeatedly resampling the data to estimate parameters or perform hypothesis tests without relying on specific distributional assumptions.

8. **Advantages**: Nonparametric methods are robust and can be applied to a wide range of data types and situations, especially when assumptions about data distribution are violated.

9. **Limitations**: Nonparametric tests may have less statistical power compared to their parametric counterparts when the data truly follow a specific distribution. Additionally, they may require larger sample sizes to achieve the same level of precision.

In summary, nonparametric statistics provide valuable tools for analyzing and drawing conclusions from data that do not conform to the assumptions of parametric statistics. They are particularly useful when dealing with categorical, ordinal, or non-normally distributed data and offer a robust approach to hypothesis testing and data analysis in a variety of fields, including social sciences, biology, and engineering.

# See more
[[digital-garden/docs/Statistics/Nonparametric Methods/Advantages of Nonparametric Methods over Parametric Methods\|Advantages of Nonparametric Methods over Parametric Methods]]