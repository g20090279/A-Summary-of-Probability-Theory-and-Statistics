- Topics: Chi-square Distribution and Related Distributions
- Last Revised: June 18, 2023

---

# The Chi-Square Distribution

The Chi-squared distribution is a special case of gamma distribution. It is widely used in inferential statistics, The Chi-square distribution results when k standard normal random variables are squared and summed,

> **Definition**. If $X_1,\dots,X_k$ are independent standard normal random variables (standard indicates mean 0 and variance 1, denoted as $X_i\sim\mathcal{N}(0,1)$ for $i=1,\dots,k$), then the sum of their squares
>$$Q=\sum_{i=1}^{k}X_i^2$$
>is distributed as Chi-squared distribution with $k$ degrees of freedom, which is denoted as
>$$Q\sim\chi^2_k.$$

## Probability Density Function (PDF)

The formula for the probability density function (PDF) of the Chi-square distribution is (Dodge, 2008)

> $$f(x)=\frac{e^{-\frac{x}{2}}x^{\frac{k}{2}-1}}{2^{\frac{k}{2}}\Gamma\left(\frac{k}{2}\right)},\quad x\geq0,$$

where $k$ is any positive integer, and the gamma function is defined by

$$\Gamma(k)=\int_0^{\infty} t^{k-1}e^{-t}\ dt,\quad t>0.$$

The PDF of Chi-square distribution can be derived by the relation to the normal distributions.

### Properties of the Gamma Function

We can rewrite the gamma function by integration by parts ($\int udv=uv-\int vdu$), where $u=t^{k-1}$ and $v=-e^{-t}$, resulting in

$$\Gamma(k)=\left.-t^{k-1}e^{-t}\right\lvert_0^\infty-\int_0^\infty -e^{-t}(k-1)t^{k-1}dt.$$

The first term on the right-hand side equals 0, which can be calculated by repetitively applying $k-1$ times L'Hopital's rule. The above equation can be written as

$$\Gamma(k)=(k-1)\Gamma(k-1).$$

Repetitively applying this recurrence relation, we have

> $$\Gamma(k)=(k-1)!\Gamma(1)=(k-1)!$$

Note that $\Gamma(1)=\int_0^\infty e^{-x}dx=1.$

## Cumulative Distribution Function (PDF)

## Properties

# Related Distributions

## The Non-Central Chi-Square Distribution

Much of the importance of the Chi-square distribution stems from the fact that it is the distribution that governs the sum of squares of independent, standard normal variables. A natural generalization and one that is important in statistical applications, is to consider the distribution of a sum of squares of independent normal variables, each with variance 1 but with different means.

## Sum of Squares of Normal Distribution with Zero Mean But Not Unit Variance

The Chi-square distribution results from the sum of serval normal random variables which must have zero mean and unit variance. What if the normal variables have zero mean but not unit variance? Assume that the $i$-th random variable $X_i\sim\mathcal{N}(0,\sigma_i^2)$.

One simplified case is that the variances of all independent random variables are the same, which can be denoted as $\sigma_i^2=\sigma^2$. To transform a zero mean variance $\sigma^2$ $X_i\sim\mathcal{N}(0,\sigma^2)$ to a standard normal $X_i^\prime\sim\mathcal{N}(0,1)$, we can simply scale $X_i$ as

$$X_i^\prime=\frac{1}{\sigma}X_i,$$

and therefore the sum of squares are related as

$$P=\sum_{i=1}^{k}X_i^2=\sigma^2\sum_{i=1}^{k}(X_i^{\prime})^2.$$

Note that if the PDF for random variable $Z$ is $f_Z(z)$, then the scaled random variable $c\cdot Z$ has CDF

$$\text{Pr}\left\{c\cdot Z<z\right\}=\text{Pr}\left\{Z<\frac{z}{c}\right\}=F_Z(\frac{z}{c})$$

and the PDF

$$\frac{d}{dz}\left[F_Z\left(\frac{z}{c}\right)\right]=\frac{1}{c}f_Z\left(\frac{z}{c}\right).$$

In a conclusion, the sum of squares of $k$ independent normal random variables with zero mean and variance $\sigma^2$, which is denoted as $P$, has PDF

$$f_P(x)=\sigma^2f_{\chi^2}(\sigma^2\cdot x).$$

# References


