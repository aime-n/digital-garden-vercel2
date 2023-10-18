---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/non-parametric-tests/"}
---



# Non parametric Methods


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/nonparametric-methods/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




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

</div></div>


## Non parametric Tests

### Wilcoxon Test


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/wilcoxon-test/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




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





</div></div>


### Chi-Squared Test

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/chi-squared/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





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
$
\chi^2 = \sum \frac{(O_i - E_i)^2}{E_i}
$

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

</div></div>


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/chi-squared-test-application/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





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



</div></div>

### Teste de Corrida


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/teste-de-corrida/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# Run Test Procedure

Follow the steps below to execute the run test, which is used to determine whether a sequence of symbols occurs randomly and independently.

### 1) **Formulate the Hypotheses**
   - **Null Hypothesis ( $H_0$ ):** Symbols in the sequence occur randomly and independently, without significant run patterns.
   - **Alternative Hypothesis ( $H_1$ ):** Symbols in the sequence do not occur randomly, indicating the presence of significant run patterns.

### 2) **Count Observed Runs**
   - The sequence contains four runs of A and four runs of B. A run of A consists of several consecutive A's until there is a switch to B, and vice versa for a run of B.
   - $r =$ total number of runs, i.e., how many times it switched to each symbol.

### 3) **Calculate Expected Runs**
   - Under the null hypothesis of randomness, the expected number of runs can be calculated using the Wald-Wolfowitz formula:
     $R_{\text{exp}} = 1 + \frac{2n_1n_2}{n_1 + n_2}$
     where:
     - $R_{\text{exp}} =$ expected number of runs.
     - $n_1 =$ number of symbols of A.
     - $n_2 =$ number of symbols of B.

### 4) **Calculate Variance of $R$**
   - Details for calculating the variance should be included here.

### 5) **Standardize Number of Runs and Obtain $z$**
   - Details for standardizing and obtaining $z$ should be included here.

### 6) **Comparison with Critical $z$ Value (1.96)**
   - If $|z| < |z_{\text{crit}}|$, we do not reject the hypothesis of randomness (1.96 is used assuming a 5% significance level for a two-tailed test).


</div></div>



### Kolmogorov Smirnov Test

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/kolmogorov-smirnov/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





# Kolmogorov-Smirnov Test Procedure

>[!info] Definition
>The Kolmogorov-Smirnov (K-S) test is utilized for continuous data to test the goodness of fit, determining whether a sample follows a specific distribution.

## **Procedure Steps:**

### **1) Formulate the Hypotheses**
   - **Null Hypothesis ( $H_0$ ):** The sample follows distribution X.
   - **Alternative Hypothesis ( $H_1$ ):** The sample does not follow distribution X.

### **2) Order Data and Construct a Table**
   - Order the data in ascending order.
   - Calculate the Empirical Cumulative Distribution Function (ECDF) and the theoretical CDF.
#### ECDF

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/calculo-da-distribuicao-acumulada-empirica-ecdf/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




A Distribuição Acumulada Empírica (ECDF, sigla em inglês para Empirical Cumulative Distribution Function) é uma função estatística que **descreve a distribuição cumulativa** dos dados em um conjunto de amostras. Ela é usada para representar graficamente como os dados estão distribuídos em relação a uma variável aleatória e é uma maneira empírica de estimar a função de distribuição acumulada de uma população a partir de dados amostrais.

A ECDF é construída da seguinte maneira:

1. Ordene os dados em ordem crescente.

2. Para cada valor de dados na amostra, calcule a proporção de valores iguais ou menores a ele na amostra. Isso é feito dividindo o número de valores menores ou iguais ao valor atual pelo tamanho total da amostra.

3. Crie um gráfico de dispersão onde o eixo x representa os valores dos dados e o eixo y representa as proporções calculadas no passo 2.

A ECDF é uma representação acumulativa da distribuição dos dados e é útil para visualizar como os dados estão distribuídos em relação a uma variável aleatória. Ela permite que você identifique rapidamente características importantes da distribuição, como a mediana, os quartis e a forma geral da distribuição.

A ECDF é uma ferramenta valiosa na análise exploratória de dados, especialmente quando você deseja entender a distribuição de seus dados sem fazer suposições específicas sobre a forma da distribuição subjacente. É frequentemente usada em estatística descritiva e em gráficos de probabilidade, como o gráfico de probabilidade normal, que é usado para verificar se os dados seguem uma distribuição normal.

</div></div>

   
   **Columns of the Table:**
   - $x$: Value, ordered from smallest to largest.
   - **Order:** From 1 to the sample size.
   - $Fn(x)$: Order/n (ECDF).
   - $F0(x)$: Theoretical CDF, calculate the integral of the probability density function (pdf).
   - $|F0(x) - Fn(x)|$: $D_n$.
   - $|F0(x) - Fn(x-)|$: Crossed $D_n$.  --> subtrai o Fn da linha anterior



### **3) Find the Maximum Deviation, $d$, Value**
   - Look for $d$, i.e., the maximum value of the last two columns.

### **4) Comparison with Critical Values**
   - Compare the calculated $d$ value with the critical values given in the K-S test table, and identify the $p-value$ range.
   - If the $p-value > 0.05$, we do not reject the null hypothesis $H_0$.

   **Example for Uniform Distribution PDF:**
   - $PDF$: $(x+1)/2$



</div></div>


## Wilcoxon Test
!
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/wilcoxon-test/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




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





</div></div>
 ou 
<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




The Wilcoxon Rank-Sum Test, also known as the Mann-Whitney U Test, is a nonparametric statistical test used to determine whether there is a statistically significant difference between two independent groups or samples. 

In essence, this test assesses whether the two groups have similar distributions or whether one tends to have consistently higher or lower values compared to the other. It accomplishes this by ranking all the values from both groups together, then summing the ranks of one group, and comparing this sum to the expected sum under the null hypothesis (which assumes no difference between groups).

The Wilcoxon Rank-Sum Test is particularly useful when dealing with [[digital-garden/docs/Statistics/Data Analysis and Visualization/Data Type/Ordinal Data\|Ordinal Data]], skewed, or non-normally distributed data and when the assumptions of parametric tests like the t-test cannot be met. It is widely used in various fields, including biology, social sciences, and clinical research, to compare groups in situations where a simple comparison of means might not be appropriate or valid.

</div></div>




### Sign Test

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/digital-garden/docs/statistics/nonparametric-methods/sign-test/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# FISCHER SIGN TEST

- **Data Characteristics:**
   - Continuous
   - Independent
   - Single median equal to the parameter theta

>[!info] Definition
>The Sign Test is a non-parametric statistical method used to analyze the median of a single sample or to compare the medians of two paired samples. 

It’s particularly helpful when the assumptions of parametric tests, like t-tests, are not met (e.g., normality). Below is a comprehensive overview of the Sign Test:

### **Sign Test**

#### **Application:**

- **Single Sample**: Testing whether the median of a single sample is equal to a specified value.
- **Paired Samples**: Testing whether there is a difference in the medians of two paired samples.

#### **Key Concepts:**

- **Data Type:** The test uses ordinal, interval, or ratio data.
- **Null Hypothesis (\(H_0\)):** Assumes no difference in medians or that the median difference is zero.
- **Alternative Hypothesis (\(H_1\)):** Assumes a significant difference in medians or that the median difference is not zero.

#### **Advantages:**

- **Robust:** Less sensitive to outliers and non-normal data.
- **Flexibility:** Suitable for small sample sizes.

#### **Disadvantages:**

- **Sensitivity:** Less powerful than parametric tests like the t-test, meaning it might not detect differences that actually exist.

#### **Example:**

Suppose we are analyzing the effects of a training program by comparing the pre-test and post-test scores of participants.

1. **Hypotheses:**
   - \(H_0: \text{median difference} = 0\)
   - \(H_1: \text{median difference} \neq 0\)

2. **Differences and Signs:**
   - Calculate differences (post-test - pre-test) and assign signs.

3. **Test Statistic:**
   - Count the number of positive differences.

4. **Decision:**
   - Compare the count to a critical value or calculate the p-value to make a decision regarding the null hypothesis.

Using the Sign Test provides a non-parametric alternative to analyze and interpret the central tendency of datasets or the difference between paired datasets.


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



#### **Procedure:**
1. **Formulate Hypotheses:**
   - **H0:** No differences in the medians.
   - **H1:** There are differences in the medians.

2. **Determine Differences:**
   - For paired samples, calculate the differences between paired observations.
   - Disregard any pairs where the difference is zero.

3. **Assign Signs:**
   - Assign a positive sign to positive differences and a negative sign to negative differences.

4. **Calculate Test Statistic:**
   - The test statistic is the number of positive differences.
   - If there's a null difference (difference = 0), it is eliminated, and the sample size $n$ becomes $n - 1$, and so on.

   **"Two-Tailed Hypothesis Test for a Binomial Distribution."**

   $p\text{-value} = \sum_{j=B_{obs}}^{n} P_0(B \geq B_{obs}), \text{ where } B \sim \text{binomial}(n, 1/2).$

   $p\text{-value} = 1 - \text{BinomialCDF}(n, p=1/2, k=B_{obs} - 1)$
Where:
$n$: number of trials
$p$: probability of success in a single trial
$k$: number of successess. By using $B_{obs}​−1$, we ensure that we are looking at the tail probability beyond the observed value, not including it.

5. **Decision:**

   - Compare the test statistic to a critical value from a binomial distribution or calculate a p-value.
   - Decide whether to reject or fail to reject the null hypothesis based on a significance level (e.g., α = 0.05).

   - Reject or fail to reject.
   - If $p\text{-value} > 0.05$, fail to reject $H_0$.



</div></div>




</div></div>


