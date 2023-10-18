---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/nonparametric-methods/teste-de-corrida/"}
---

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
