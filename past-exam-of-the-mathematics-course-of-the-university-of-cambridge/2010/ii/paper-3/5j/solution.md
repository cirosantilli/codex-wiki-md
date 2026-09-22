<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Assume $n>p\ge1$, the ordinary nonsaturated [Gaussian linear model](../../../../../normal-linear-model.md). The log [likelihood](../../../../../likelihood-function.md) is, up to a constant,

$$
\ell(\beta,\sigma^2)=-\frac n2\log\sigma^2-\frac{\|Y-X\beta\|^2}{2\sigma^2}.
$$

The normal equations and full column rank give the [least-squares estimator](../../../../../ordinary-least-squares-estimators.md) $\widehat\beta=(X^TX)^{-1}X^TY$. Write $H=X(X^TX)^{-1}X^T$ and $Q=I-H$, an [orthogonal projection](../../../../../orthogonal-projection.md) of rank $n-p$. Maximizing in $\sigma^2$ yields

$$
\boxed{\widehat\sigma^2=\frac{Y^TQY}{n}.}
$$

Since $QX=0$, the residual sum of squares is $\varepsilon^TQ\varepsilon$. Expanding its [expectation](../../../../../expected-value.md) uses only $\mathbb E\varepsilon_i\varepsilon_j=\sigma^2\delta_{ij}$:

$$
\mathbb E(Y^TQY)=\sum_{i,j}Q_{ij}\mathbb E(\varepsilon_i\varepsilon_j)
=\sigma^2\operatorname{tr}Q=(n-p)\sigma^2.
$$

This does not use [Cochran's theorem](../../../../../cochran-s-theorem.md). It proves bias $-p\sigma^2/n$ and gives

$$
\boxed{\mathbb E\widehat\sigma^2=(1-p/n)\sigma^2,\qquad
\widetilde\sigma^2=\frac{Y^TQY}{n-p},\qquad\mathbb E\widetilde\sigma^2=\sigma^2.}
$$

In the saturated case $n=p$, residuals vanish identically, the likelihood is unbounded as the positive [variance](../../../../../variance-split.md) tends to zero, and the unbiased residual [estimator](../../../../../estimator.md) is unavailable. Thus the usual variance-estimation request requires $n>p$.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
