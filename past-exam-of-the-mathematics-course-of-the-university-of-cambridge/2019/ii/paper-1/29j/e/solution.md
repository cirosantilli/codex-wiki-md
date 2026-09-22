<h1 id="29j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Using the estimator from part (b) and the [spectral decomposition](../../../../../../spectral-decomposition.md) of $X^TX$,

$$
\widehat Y_\lambda
=XV(\Lambda+\lambda I_p)^{-1}V^TX^TY
=U(\Lambda+\lambda I_p)^{-1}U^TY.
$$

Thus

$$
\boxed{\widehat Y_\lambda=U(\Lambda+\lambda I_p)^{-1}U^TY
=\sum_{i=1}^p\frac{\Lambda_{ii}}{\Lambda_{ii}+\lambda}w_iw_i^TY.}
$$

Under the stated separation of scales, the shrinkage factor is approximately one for $i\leq q$ and approximately zero for $i>q$. The [principal-component shrinkage by ridge regression](../../../../../../principal-component-shrinkage-by-ridge-regression.md) formula therefore reduces approximately to

$$
\widehat Y_\lambda\approx\sum_{i=1}^q w_iw_i^TY,
$$

the [orthogonal projection](../../../../../../orthogonal-projection.md) of $Y$ onto the span of the $q$ normalized sample principal components with greatest variance.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
