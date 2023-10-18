---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/chi-squared-test-application/"}
---


### Application

- **Goodness-of-Fit Test:**
  Used to determine if the sample data fits a specific distribution. It compares the observed frequencies to the expected frequencies of a particular categorical variable.

- **Test of Independence:**
  Used to assess whether two categorical variables are independent of each other. It evaluates the dependence between the variables in a contingency table.

- **Test of Homogeneity:**
  Used to determine if different samples come from the same population. It examines whether the distribution of sample characteristics is consistent across different populations.

# Case
# Example of Chi-Square Test

## Objective

Investigate whether there is a significant relationship between smoking habits (Smoker/Non-Smoker) and occurrence of lung cancer.
![Pasted image 20231016050102.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016050102.png)

## Data Collection

A sample data of 500 individuals is as follows:

### Contingency Table

|            | Lung Cancer | No Lung Cancer | Total |
|:---------- |:----------- |:-------------- |:----- |
| Smoker     | 100         | 150            | 250   |
| Non-Smoker | 30          | 220            | 250   |
| Total      | 130         | 370            | 500      |

## Calculation

1. **Expected Frequencies**  
   $E_{ij} = \frac{(Row Total_i) \times (Column Total_j)}{(Grand Total)}$
   

2. **Chi-Square Statistic**  
   $\chi^2 = \sum \frac{(O_{ij} - E_{ij})^2}{E_{ij}}$  
   Where $O_{ij}$ represents the observed frequency and $E_{ij}$ represents the expected frequency.
![Pasted image 20231016041819.png|250x200](/img/user/Bins/att/Pasted%20image%2020231016041819.png)
![Pasted image 20231016045919.png|250x200](/img/user/Bins/att/Pasted%20image%2020231016045919.png)


## Graph
![Pasted image 20231016050142.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016050142.png)


![Pasted image 20231016050345.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016050345.png)
## Hypotheses

- Null Hypothesis ($H_0$): There is no association between smoking and lung cancer.
- Alternative Hypothesis ($H_1$): There is an association between smoking and lung cancer.

## Results and Conclusion

- If the **calculated Chi-Square value** is greater than the critical value (for a specific alpha level, say 0.05), we reject the null hypothesis, concluding that there is a significant association between smoking and lung cancer.
- If the calculated Chi-Square value is less than the critical value, we fail to reject the null hypothesis, suggesting that the data does not provide enough evidence to conclude a significant association between smoking and lung cancer.

![Pasted image 20231016050604.png|undefined](/img/user/Bins/att/Pasted%20image%2020231016050604.png)

