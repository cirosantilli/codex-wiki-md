<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [ordinary least squares](../../../../../../ordinary-least-squares.md) estimator is $\widehat\beta=(X^TX)^{-1}X^TY$. Consequently the [fitted values](../../../../../../fitted-values.md) and [regression residuals](../../../../../../regression-residual.md) are

$$
\widehat Y=X\widehat\beta=PY,\qquad e=Y-\widehat Y=(I_n-P)Y.
$$

An affine transformation of a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) is again [multivariate normal](../../../../../../multivariate-normal-distribution.md), possibly with a singular [covariance matrix](../../../../../../covariance-matrix.md). For a [random vector](../../../../../../random-vector.md) with [covariance matrix](../../../../../../covariance-matrix.md) $\Sigma$, its transformed [covariance matrix](../../../../../../covariance-matrix.md) is $A\Sigma A^T$. Since $PX=X$, $P^2=P=P^T$ and $(I-P)^2=I-P$, these results give

$$
\boxed{\widehat Y\sim N_n(X\beta,\sigma^2P),\qquad e\sim N_n(0,\sigma^2(I_n-P)).}
$$

Both [multivariate normal distributions](../../../../../../multivariate-normal-distribution.md) are supported on their respective projected subspaces. In particular, $\widehat Y_i$ has [variance](../../../../../../variance-split.md) $\sigma^2P_{ii}$ and $e_i$ has [variance](../../../../../../variance-split.md) $\sigma^2(1-P_{ii})$; the [regression residuals](../../../../../../regression-residual.md) need not be mutually independent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
