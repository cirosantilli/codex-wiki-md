<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Let $RSS_0$ and $RSS_1$ be the residual sums of squares under the restricted model with $p_0$ coefficients and the full model with $p$ coefficients. Assuming $X$ has full column rank, the [nested-model F-test](../../../../../nested-model-f-test.md) uses

$$
\boxed{F=\frac{(RSS_0-RSS_1)/(p-p_0)}{RSS_1/(n-p)}.}
$$

Under the null hypothesis this has the $F_{p-p_0,n-p}$ distribution.

Maximizing the Gaussian likelihood over $\beta$ and the unknown variance gives $\widehat\sigma^2=RSS/n$. Thus the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md) is

$$
-2\log\Lambda=n\log\frac{RSS_0}{RSS_1}.
$$

Since

$$
\frac{RSS_0}{RSS_1}=1+\frac{p-p_0}{n-p}F,
$$

we obtain

$$
\boxed{-2\log\Lambda
=n\log\left(1+\frac{p-p_0}{n-p}F\right).}
$$

The logarithm is strictly increasing, so the two test statistics give exactly the same rejection ordering.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
