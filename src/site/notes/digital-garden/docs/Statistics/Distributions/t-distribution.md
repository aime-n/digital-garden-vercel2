---
{"dg-publish":true,"permalink":"/digital-garden/docs/statistics/distributions/t-distribution/"}
---

The **t-distribution**, also known as the Student's t-distribution, is a probability distribution that plays a crucial role in statistics, particularly in hypothesis testing when the population standard deviation is unknown and sample sizes are relatively small. The t-distribution is similar in shape to the standard normal distribution (z-distribution) but has heavier tails, making it more appropriate for small sample sizes.

Here are some key characteristics and points about the t-distribution:

1. **Shape:** The t-distribution is symmetric and bell-shaped, much like the normal distribution. However, it has thicker tails, which means it has more variability in the extreme values compared to the normal distribution.

2. **Parameter:** The t-distribution is characterized by a single parameter called **degrees of freedom (df)**. The degrees of freedom represent the sample size and play a crucial role in determining the shape of the distribution. As the degrees of freedom increase, the t-distribution approaches the normal distribution.

3. **Application:** The t-distribution is commonly used when working with small sample sizes and estimating population parameters. It is used in situations where the population standard deviation is unknown, and sample data are used to estimate it. In such cases, the sample standard deviation is used as an estimate, and the t-distribution adjusts for the uncertainty introduced by this estimation.

4. **t-Statistic:** In hypothesis testing, the t-statistic is calculated using the sample mean, population mean (or reference value), sample standard deviation, and sample size. The formula for the t-statistic is similar to the z-score formula:

   \[t = \frac{{\bar{x} - \mu}}{{s / \sqrt{n}}}\]

   - \(\bar{x}\) is the sample mean.
   - \(\mu\) is the population mean (or reference value).
   - \(s\) is the sample standard deviation.
   - \(n\) is the sample size.

5. **Degrees of Freedom:** The degrees of freedom for the t-distribution are determined by \(n - 1\), where \(n\) is the sample size. The choice of degrees of freedom impacts the shape of the distribution. As the degrees of freedom increase, the t-distribution approaches the standard normal distribution.

6. **Critical Values:** Critical values for the t-distribution are used in hypothesis testing to determine the threshold beyond which results are considered statistically significant. The critical values depend on the chosen significance level (alpha) and the degrees of freedom.

In summary, the t-distribution is a probability distribution that is particularly useful in situations where the population standard deviation is unknown, and small sample sizes are involved. It provides a way to account for the increased uncertainty associated with estimating the standard deviation from the sample data. The choice of degrees of freedom determines the specific t-distribution used in a given analysis.