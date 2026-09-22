<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Assume $X$ has full column rank. The log-likelihood, up to constants, is

$$
-\frac n2\log\sigma^2-\frac1{2\sigma^2}\|Y-X\beta\|^2.
$$

The [ordinary least squares](../../../../../ordinary-least-squares-estimators.md) normal equations give

$$
\widehat\beta=(X^TX)^{-1}X^TY,
$$

and maximizing over the variance gives the maximum-likelihood estimator

$$
\widehat\sigma^2=\frac1n\|(I-H)Y\|^2.
$$

Because $I-H$ is an orthogonal projection of rank $n-p$,

$$
\boxed{\frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p}}.
$$

Writing $\chi^2_{\nu,q}$ for the $q$-quantile, a confidence interval of level $1-\alpha$ is

$$
\boxed{\left[
\frac{n\widehat\sigma^2}{\chi^2_{n-p,1-\alpha/2}},
\frac{n\widehat\sigma^2}{\chi^2_{n-p,\alpha/2}}
\right]}.
$$

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
