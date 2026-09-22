<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [independent](../../../../../../independent-random-variables.md) Poisson counts, the [log-likelihood](../../../../../../log-likelihood.md) at mean vector $\mu$ is

$$
\ell(\mu)=\sum_i\{y_i\log\mu_i-\mu_i-\log(y_i!)\}.
$$

The saturated model maximizes each cell separately at $\widehat\mu_i=y_i$, including the boundary value zero. If $e_i$ is the fitted mean under the log-linear regression, twice the saturated-minus-fitted [log-likelihood](../../../../../../log-likelihood.md) is the full [Poisson deviance](../../../../../../poisson-deviance.md)

$$
D=2\sum_i\left\{y_i\log\frac{y_i}{e_i}-y_i+e_i\right\},
$$

with $0\log(0/e_i)=0$ understood by continuity. The fitted intercept has [score function](../../../../../../informant-function.md) $\partial\ell/\partial\mu=\sum_i(y_i-e_i)$, since differentiating the logarithmic mean with respect to that intercept gives one. Its maximum-likelihood equation therefore gives $\sum_i e_i=\sum_i y_i$. This is why [Poisson deviance simplifies when an intercept is fitted](../../../../../../poisson-deviance-simplifies-when-an-intercept-is-fitted.md):

$$
\boxed{D=2\sum_i y_i\log(y_i/e_i)}.
$$

Without the fitted unpenalized intercept, one cannot generally discard the two linear terms. The individual logarithmic terms in the simplified sum need not each be positive; nonnegativity belongs to the full [deviance](../../../../../../exponential-family-deviance.md), or to the full cell contributions before cancellation.

For the approximation, write $y_i=e_i+r_i$ and expand $\log(1+r_i/e_i)$. When relative residuals are small,

$$
\begin{aligned}
2\left\{(e_i+r_i)\log\left(1+\frac{r_i}{e_i}\right)-r_i\right\}
&=\frac{r_i^2}{e_i}-\frac{r_i^3}{3e_i^2}
+O\left(\frac{r_i^4}{e_i^3}\right).
\end{aligned}
$$

Consequently the [quadratic Pearson approximation to the Poisson deviance](../../../../../../quadratic-pearson-approximation-to-the-poisson-deviance.md) is

$$
\boxed{D\simeq\sum_i\frac{(y_i-e_i)^2}{e_i}},
$$

the [Pearson chi-squared statistic](../../../../../../pearson-chi-squared-statistic.md) for unit Poisson dispersion. Adequate expected counts and small relative residuals are what make the quadratic approximation useful; it is not an exact identity and can be poor for sparse cells, especially a zero count with positive fitted mean. Any further chi-squared goodness-of-fit reference needs its own large-count regularity assumptions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
