Topics: Chi-square Distribution
Last Revised: June 14, 2024

---

The Chi-squared distribution is a special case of gamma distribution. It is widely used in inferential statistics, The Chi-square distribution results when k standard normal random variables are squared and summed,

> **Definition**. If $X_1,\dots,X_k$ are independent standard normal random variables (standard indicates mean 0 and variance 1), then the sum of their squares
$$Q=\sum_{i=1}^{k}X_i^2$$
is distributed as Chi-squared distribution with $k$ degrees of freedom, which is denoted as
$$Q\sim\chi^2_k.$$

# Probability Density Function (PDF)

The formula for the probability density function (PDF) of the Chi-square distribution is

$$f(x)=\frac{e^{-\frac{x}{2}}x^{\frac{k}{2}-1}}{2^{\frac{k}{2}}\Gamma\left(\frac{k}{2}\right)},\quad x\geq0,$$

where the gamma function is

$$\Gamma(k)=\int_0^{\infty} t^{k-1}e^{-t}\ dt.$$

# References


