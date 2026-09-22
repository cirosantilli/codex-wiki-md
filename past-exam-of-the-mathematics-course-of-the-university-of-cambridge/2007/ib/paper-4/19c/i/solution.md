<h1 id="19c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $S_{xx}=\sum_i x_i^2$ and $\bar Y=n^{-1}\sum_iY_i$. For an identifiable two-parameter [linear regression](../../../../../../linear-regression-split.md) assume $S_{xx}>0$; for the [variance](../../../../../../variance-split.md) estimate and test below also assume $n>2$. The [least-squares normal equations](../../../../../../normal-equations-for-linear-least-squares.md) are

$$
\sum_i(Y_i-\widehat\alpha-\widehat\beta x_i)=0,\qquad\sum_i x_i(Y_i-\widehat\alpha-\widehat\beta x_i)=0.
$$

Using $\sum_i x_i=0$ gives

$$
\boxed{\widehat\alpha=\bar Y,\qquad\widehat\beta=\frac{\sum_i x_iY_i}{S_{xx}}.}
$$

The [residual sum of squares](../../../../../../residual-sum-of-squares.md) has positive-definite quadratic part $n\alpha^2+S_{xx}\beta^2$, so these equations give its unique minimum. The [normal distribution](../../../../../../normal-distribution.md) of the independent errors gives the [log-likelihood](../../../../../../log-likelihood.md)

$$
\ell(\alpha,\beta,\sigma^2)=-\frac n2\log(2\pi\sigma^2)-\frac1{2\sigma^2}\sum_i(Y_i-\alpha-\beta x_i)^2.
$$

For every fixed positive $\sigma^2$, maximizing this over $\alpha,\beta$ is exactly minimizing the same [residual sum of squares](../../../../../../residual-sum-of-squares.md). Thus the [ordinary least squares estimators](../../../../../../ordinary-least-squares-estimators.md) are also the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md).

The printed hypotheses do not explicitly require $S_{xx}>0$ or $n>2$. If $S_{xx}=0$, all $x_i$ vanish and $\beta$ is unidentifiable; this is an intercept-only model with $n-1$ residual degrees of freedom. For $n=1$ its residual is identically zero, so the likelihood has no finite maximizer with positive variance. If $S_{xx}>0$ but $n=2$, the fit is saturated, leaving no residual [variance](../../../../../../variance-split.md) estimate or Student test with positive degrees of freedom. The following nondegenerate formulas use $S_{xx}>0$ and $n>2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [19C](../../19c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
