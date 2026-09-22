<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [moving-average process of order one](../../../../../../moving-average-process-of-order-one.md), $\gamma(0)=\sigma^2(1+\theta_1^2)$, $\gamma(1)=\sigma^2\theta_1$, and $\gamma(2)=0$. Regressing each endpoint on the single intervening observation leaves residual [covariance](../../../../../../covariance.md) $\gamma(2)-\gamma(1)^2/\gamma(0)$ and residual [variance](../../../../../../variance-split.md) $\gamma(0)-\gamma(1)^2/\gamma(0)$. Therefore its lag-two [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) is

$$
\alpha(2)=\frac{\rho(2)-\rho(1)^2}{1-\rho(1)^2}
=\boxed{-\frac{\theta_1^2}{1+\theta_1^2+\theta_1^4}.}
$$

The denominator is positive. In particular, the moving-average autocorrelation cutoff at lag one does not make the lag-two partial correlation zero unless $\theta_1=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
