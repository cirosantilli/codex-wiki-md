<h1 id="29j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Since $X=UV^T$ and $X^TX=V\Lambda V^T$,

$$
\widehat Y_{\rm MLE}
=X(X^TX)^{-1}X^TY
=U\Lambda^{-1}U^TY.
$$

Therefore

$$
\boxed{\widehat Y_{\rm MLE}=U\Lambda^{-1}U^TY.}
$$

Put $w_i=u_i/\sqrt{\Lambda_{ii}}$. By part (c), the $w_i$ are [normalized sample principal components](../../../../../../normalized-sample-principal-component.md) forming an [orthonormal set](../../../../../../orthonormal-set.md), and

$$
U\Lambda^{-1}U^T=\sum_{i=1}^p w_iw_i^T.
$$

This is the [orthogonal projection onto a finite-dimensional subspace](../../../../../../orthogonal-projection-onto-a-finite-dimensional-subspace.md) spanned by the $w_i$, so $\widehat Y_{\rm MLE}$ is the unique closest point in that subspace to $Y$.

## ↑ Ancestors (11)

1. [D](../d.md)
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
