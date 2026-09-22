<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

The normal-model [log-likelihood](../../../../../log-likelihood.md) is $-\frac n2\log\sigma^2-\|Y-X\beta\|^2/(2\sigma^2)$ up to a constant. Differentiating gives the [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad
\widehat\sigma^2=\frac1n\|Y-X\widehat\beta\|^2.}
$$

Let $P=X(X^TX)^{-1}X^T$. The fitted component $P\varepsilon$ and residual $(I-P)\varepsilon$ are orthogonal jointly normal projections and hence independent. Therefore

$$
\widehat\beta\sim N_p(\beta,\sigma^2(X^TX)^{-1}),\qquad
\frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p},
\qquad \widehat\beta\ \text{and}\ \widehat\sigma^2\text{ are independent}.
$$

The prediction error $\widetilde y-y^*=x^{*T}(\widehat\beta-\beta)-\varepsilon^*$ is normal with mean zero and variance $\sigma^2\tau^2$, and is independent of the residual variance estimate. Dividing by the independent estimated standard deviation yields

$$
\boxed{\frac{\widetilde y-y^*}{\widetilde\sigma\tau}\sim t_{n-p}.}
$$

Thus the [prediction interval in a normal linear model](../../../../../prediction-interval-in-a-normal-linear-model.md) is

$$
\boxed{\widetilde y\ \pm\ t_{n-p,1-\alpha/2}\,\widetilde\sigma
\sqrt{1+x^{*T}(X^TX)^{-1}x^*}.}
$$

The extra $1$ includes the new observation's independent noise; omitting it would give a confidence interval for its conditional mean instead.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
