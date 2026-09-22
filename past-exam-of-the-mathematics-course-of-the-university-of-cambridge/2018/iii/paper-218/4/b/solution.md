<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The null model has only an intercept:

$$
Y_i\overset{\mathrm{iid}}\sim\operatorname{Poisson}(\mu),\qquad\log\mu=\beta_0.
$$

For $\bar Y>0$, maximizing its [log-likelihood](../../../../../../log-likelihood.md) gives $\widehat\mu=\bar Y$ and $\widehat\beta_0=\log\bar Y$. The saturated [Poisson regression](../../../../../../poisson-regression.md) gives each observation its own fitted mean $\widehat\mu_i=Y_i$, allowing zero as a limiting fitted mean. By the definition of [Poisson deviance](../../../../../../poisson-deviance.md),

$$
D_0=2\sum_{i=1}^{107}\left\{Y_i\log\frac{Y_i}{\bar Y}-(Y_i-\bar Y)\right\}.
$$

Since $\sum_i(Y_i-\bar Y)=0$,

$$
\boxed{D_0=2\sum_{i=1}^{107}Y_i\log(Y_i/\bar Y).}
$$

Use the continuous convention $0\log(0/\bar Y)=0$. If all counts are zero, both the saturated and null likelihood maxima are attained as limits at zero mean and the deviance is zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
