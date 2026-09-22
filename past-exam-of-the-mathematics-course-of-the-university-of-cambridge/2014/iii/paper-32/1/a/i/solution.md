<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a one-sided [Wald test](../../../../../../../wald-test.md) use the [signed normal Wald statistic](../../../../../../../signed-normal-wald-statistic.md), rather than its square. The [maximum-likelihood estimate](../../../../../../../maximum-likelihood-estimator.md) is the [sample mean](../../../../../../../sample-mean.md) $\bar Y_n$, with exact [variance](../../../../../../../variance-split.md) $\sigma^2/n$, so

$$
\boxed{W_n=\frac{\bar Y_n}{\sigma/\sqrt n}=\frac{\sum_{i=1}^nY_i}{\sigma\sqrt n}.}
$$

A sum of independent [normal random variables](../../../../../../../gaussian-random-variable.md) is normal, giving $\bar Y_n\sim N(\delta,\sigma^2/n)$ and hence $W_n\sim N(\sqrt n\delta/\sigma,1)$. Under the [null hypothesis](../../../../../../../null-hypothesis.md) its mean is zero:

$$
\boxed{W_n\mid\delta=0\sim N(0,1).}
$$

Thus its null distribution is exactly the [standard normal distribution](../../../../../../../standard-normal-distribution.md), without an asymptotic approximation. If the squared [Wald statistic](../../../../../../../wald-test.md) convention is used, $W_n^2$ has a [chi-squared distribution](../../../../../../../chi-squared-distribution.md) with one degree of freedom; the signed form is needed to distinguish the two directions.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
