---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/distributions/bernoulli-distribution/"}
---

Desculpe pela confusão anterior. Aqui está a correção com cifrões simples para as fórmulas inline e cifrões duplos para as fórmulas em destaque:

## **Bernoulli Distribution: Mini Wiki**

### **Overview**
The Bernoulli Distribution is a discrete probability distribution of a random variable which takes the value 1 (success) with probability $p$ and the value 0 (failure) with probability $q = 1 - p$. This distribution represents the behavior of a single experiment where the outcome is binary, often termed as a "success/failure" or "yes/no" experiment.

### **Parameters**
- $p$: Probability of success on any given trial ( $0 \leq p \leq 1$ )
- $q$ or $1 - p$: Probability of failure on any given trial

### **Probability Mass Function (PMF)**
The PMF of the Bernoulli distribution is given by:
$$ P(X=k) = \begin{cases} 
p & \text{if } k = 1, \\
1 - p & \text{if } k = 0.
\end{cases} $$

### **Expectation and Variance**
- **Expected Value (Mean)**: $\mu = p$
- **Variance**: $\sigma^2 = p(1 - p)$

### **Applications**
1. **Quality Control**: Used in manufacturing processes to analyze the probability of defective items.
2. **Finance**: Useful in modeling binary outcomes such as the movement of stock prices.
3. **Healthcare**: Applied to study the probability of the presence or absence of a disease.

### **Properties**
- The Bernoulli distribution is a special case of the Binomial distribution where $n = 1$.
- It can be used as a building block for other more complex probability distributions.
  
### **Related Distributions**
- **Binomial Distribution**: Sum of $n$ independent Bernoulli trials.
- **Geometric Distribution**: Number of Bernoulli trials needed to get one success.

### **Usage in Statistics and Data Science**
- Often used in logistic regression as it models binary outcome variables.
- Employed for hypothesis testing concerning proportions.
  
### **Limitations**
- Limited to modeling experiments with **only two possible outcomes**.

### **Conclusion**
The Bernoulli Distribution provides a mathematical framework for analyzing experiments with binary outcomes. Its simplicity makes it a foundational concept in probability theory and statistics, serving as a starting point for understanding more complicated distributions and models.

For deeper understanding, one can explore textbooks on probability and statistics, or reliable online educational resources.