---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/wilcoxon-test/","tags":["nonparametric"]}
---

The Wilcoxon Rank-Sum Test, also known as the Mann-Whitney U Test, is a non-parametric statistical hypothesis test used to compare two independent samples. It is used to determine if there are statistically significant differences between the two groups of an independent variable on a continuous or ordinal dependent variable.

![Pasted image 20231016050952.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016050952.png)

![Pasted image 20231016051051.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016051051.png)
## Characteristics of the Test:

- **[[digital-garden/docs/Statistics/Inference/Independence of Observations\|Independence of Observations]]**: The two samples being compared must be independent of each other. This means that the observations in one sample should not influence the observations in the other sample.

- **[[Continuous Data\|Continuous Data]]**: The data being analyzed should be at least ordinal, which means it should have a clear order. Continuous data can be ranked without any ties.

- **[[digital-garden/docs/Statistics/Distributions/Symmetry\|Symmetry]]**: The test assumes that the distributions of both groups are symmetrical about a common median, theta. It's important to note that the test doesn't assume that the data follows a normal distribution, just that it is symmetric about a median.

## Application:
 
The Wilcoxon Rank-Sum Test is especially useful *when the data does not meet the assumptions of a t-test*, mainly the assumption of normally distributed data. The test ranks the data and then checks for statistically significant differences in the ranks between the two groups.

To conduct the test, the data from both groups is combined and ranked together. The ranks of the data from one of the groups is then summed and compared to a distribution of summed ranks from randomly generated samples of the same sizes. This gives a test statistic which can be compared to a critical value or used to compute a p-value.

If the p-value is below a predetermined threshold (e.g., 0.05), then the difference between the groups is deemed statistically significant.

---

Note: The Wilcoxon Rank-Sum Test should not be confused with the Wilcoxon Signed-Rank Test, which is used for paired samples. The Rank-Sum Test is specifically for independent samples.



