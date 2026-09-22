<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the Gaussian sampling model $Y\mid\beta\sim N(X\beta,\sigma^2I_n)$ with known $\sigma^2>0$, and the independent prior $\beta\sim N(0,\tau^2I_p)$ with $\tau^2>0$. A Gaussian prior alone is not enough to imply the ridge result without this likelihood assumption. The [posterior distribution](../../../../../../bayesian-posterior.md) is proportional to

$$
\exp\left[-\frac1{2\sigma^2}\|Y-X\beta\|_2^2-\frac1{2\tau^2}\|\beta\|_2^2\right].
$$

Maximizing it is equivalent to minimizing the ridge objective with $\lambda=\sigma^2/\tau^2$. More explicitly, complete the square. The posterior precision, [covariance matrix](../../../../../../covariance-matrix.md) and mean are

$$
V^{-1}=\frac{X^TX}{\sigma^2}+\frac{I_p}{\tau^2},\qquad V=\sigma^2(X^TX+\lambda I_p)^{-1},\qquad m=V\frac{X^TY}{\sigma^2}=(X^TX+\lambda I_p)^{-1}X^TY.
$$

Consequently the [Gaussian posterior representation of ridge regression](../../../../../../gaussian-posterior-representation-of-ridge-regression.md) is

$$
\boxed{\beta\mid Y\sim N(m,V),\qquad \lambda=\frac{\sigma^2}{\tau^2},\qquad\operatorname{mode}(\beta\mid Y)=\mathbb E(\beta\mid Y)=\widehat\beta_\lambda.}
$$

A tighter prior, smaller $\tau^2$, implies stronger shrinkage; larger observation-noise variance at fixed prior scale also increases the penalty. The posterior covariance is $V$, not the frequentist sampling covariance of the ridge estimator, which is $\sigma^2(X^TX+\lambda I)^{-1}X^TX(X^TX+\lambda I)^{-1}$. If an intercept is to remain unpenalized, give only the slopes this proper Gaussian prior and center the design and responses.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
