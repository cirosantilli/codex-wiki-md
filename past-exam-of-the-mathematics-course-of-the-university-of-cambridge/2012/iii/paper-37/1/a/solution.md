<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [normal linear model](../../../../../../normal-linear-model.md) $Y=X\beta+\varepsilon$, with fixed full-column-rank [design matrix](../../../../../../design-matrix.md) $X$, independent errors $\varepsilon_i\sim N(0,\sigma^2)$, and $\sigma^2>0$. Its [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta,\sigma^2)=-\frac n2\log(2\pi\sigma^2)-\frac{(Y-X\beta)^T(Y-X\beta)}{2\sigma^2}.
$$

For fixed $\sigma^2$, differentiating with respect to $\beta$ gives $X^T(Y-X\widehat\beta)=0$. Since $X^TX$ is positive-definite, the unique least-squares estimate is

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

Let $\operatorname{RSS}=\|Y-X\widehat\beta\|^2$. The [variance](../../../../../../variance-split.md) score equation is $-n/(2\sigma^2)+\operatorname{RSS}/(2\sigma^4)=0$, giving

$$
\boxed{\widehat\sigma^2_{\rm ML}=\operatorname{RSS}/n.}
$$

This is the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md), whereas the [residual standard error](../../../../../../residual-standard-error.md) reported by linear-regression software is $s=\sqrt{\operatorname{RSS}/(n-p)}$. The latter uses the unbiased [residual estimate of Gaussian noise variance](../../../../../../residual-estimate-of-gaussian-noise-variance.md). These formulas assume $n>p$ and positive RSS; exact interpolation gives a [variance](../../../../../../variance-split.md)-boundary degeneracy rather than an interior maximum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
