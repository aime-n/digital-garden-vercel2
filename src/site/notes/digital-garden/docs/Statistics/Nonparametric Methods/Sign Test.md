---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/sign-test/","tags":["nonparametric"]}
---

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


