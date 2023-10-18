---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/chi-squared/","tags":["nonparametric"]}
---


![Pasted image 20231016041915.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016041915.png)

## Chi-Squared Test as a Non-Parametric Method: Mini Wiki

The Chi-Square Test is a statistical tool utilized for analyzing categorical and discrete data, commonly applied in tests of independence and randomness. Here is a structured representation of the procedure:

[[Procedure\|Procedure]]

[[digital-garden/docs/Statistics/Nonparametric Methods/Chi Squared Test - Application\|Chi Squared Test - Application]]
### Overview

>[!info] Definition:
>The Chi-Squared test, represented as χ² test, is a non-parametric statistical method used to determine if there is a significant association between two categorical variables in a sample. 

Being **non-parametric** means that it does not assume a specific distribution for the data, making it versatile and applicable to various types of categorical data. The test is widely used in research for hypothesis testing, especially in the fields of biology, marketing, sociology, and medicine.

### How It Works

1. **Observed Frequencies:**
   The first step involves counting the observed frequencies of occurrences in various categories or classes. These observations are arranged in a contingency table.

2. **Expected Frequencies:**
   Calculate the expected frequencies assuming that there is no association between the variables. The expected frequency is what you would expect if the null hypothesis were true.

3. **Calculating the Chi-Squared Statistic:**
$$
\chi^2 = \sum \frac{(O_i - E_i)^2}{E_i}
$$

   Where $O_i$ represents the observed frequency and $E_i$ represents the expected frequency.

[[digital-garden/docs/Statistics/Nonparametric Methods/Chi Squared Test - Application\|Chi Squared Test - Application]]

### Assumptions and Conditions

- **[[Categorical Data\|Categorical Data]]:**
  The Chi-Squared test is applied on categorical (nominal or ordinal) data, not on continuous data.

- **[[digital-garden/docs/Statistics/Sampling/Sample\|Sample]] Size:**
  A sufficient sample size is required, and it is suggested that the expected frequency should be 5 or more in each category.

- **[[digital-garden/docs/Statistics/Inference/Independence of Observations\|Independence of Observations]]:**
  The observations should be independent of each other, meaning that one observation should not influence another.

### Interpretation

- **[[digital-garden/docs/Statistics/Inference/Hypothesis testing/P-Value\|P-Value]]:**
  The result of the Chi-Squared test is usually interpreted using a p-value. If the p-value is below a threshold (commonly 0.05), the null hypothesis is rejected, indicating a significant association between the variables.

### Conclusion

The Chi-Squared test is a powerful non-parametric method to analyze categorical data, assessing relationships, and the goodness of fit in observed frequencies. Proper application and interpretation of the Chi-Squared test can provide valuable insights into the data, facilitating informed decision-making in research and various fields.