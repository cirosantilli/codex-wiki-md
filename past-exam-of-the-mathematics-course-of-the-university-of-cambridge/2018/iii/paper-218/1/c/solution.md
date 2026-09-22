<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Z_{ir}=\mathbf1_{\{\text{observation }i\text{ belongs to rat }r\}}$. After integrating out the [random intercepts](../../../../../../random-intercept.md),

$$
Y\sim N_{176}(X\beta,V),\qquad V=\tau^2ZZ^T+\sigma^2I_{176}.
$$

The fixed-effect [design matrix](../../../../../../design-matrix.md) has four independent columns, so the given $A$ has dimensions $176\times172$, with $A^TA=I_{172}$ and $A^TX=0$. Consequently the error contrasts $U=A^TY$ have a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) with mean zero and [covariance matrix](../../../../../../covariance-matrix.md) $W=A^TVA$.

The [restricted likelihood from orthogonal error contrasts](../../../../../../restricted-likelihood-from-orthogonal-error-contrasts.md) is their density. Equivalently, the estimates maximize

$$
\boxed{\ell_R(\tau^2,\sigma^2)=-\frac{172}{2}\log(2\pi)-\frac12\log\det W-\frac12Y^TAW^{-1}A^TY,\qquad\tau^2\geq0,\quad\sigma^2>0.}
$$

This is [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md), not maximization over individual rat effects. The unknown $\beta$ disappears because $A^TX=0$. Replacing $A$ by $AQ$ for an orthogonal $Q$ rotates $U$ and conjugates $W$, preserving the [determinant](../../../../../../determinant.md) and quadratic form; hence the objective is independent of the chosen [orthonormal basis](../../../../../../orthonormal-basis.md). The software's integrated REML log-likelihood can differ by an additive constant depending only on $X$, which has no effect on these variance estimates.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
