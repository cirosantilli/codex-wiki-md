<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Classical multidimensional scaling](../../../../../../classical-multidimensional-scaling.md) begins with a symmetric [dissimilarity matrix](../../../../../../dissimilarity-matrix.md) $D$, rather than necessarily with measured coordinates. Its aim is to find a low-dimensional Euclidean configuration representing those dissimilarities. Square the entries, not the matrix product, and define

$$
J=I-\frac1n\mathbf1\mathbf1^T,\qquad B=-\frac12J D^{(2)}J.
$$

For centered coordinates $X$, squared [Euclidean distances](../../../../../../euclidean-distance.md) satisfy $D_{ij}^2=B_{ii}+B_{jj}-2B_{ij}$ with $B=XX^T$. Multiplication on both sides by $J$ annihilates the two single-index terms, proving the double-centering formula.

If $B$ is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md), use its [spectral decomposition](../../../../../../spectral-decomposition.md) $B=U\Lambda U^T$ to construct

$$
\boxed{X_q=U_q\Lambda_q^{1/2}.}
$$

Keeping all positive [eigenvalues](../../../../../../eigenvalue.md) reproduces the original [Euclidean distances](../../../../../../euclidean-distance.md) exactly; their number is the minimal embedding dimension. Keeping fewer gives a low-rank approximation to the [Gram matrix](../../../../../../gram-matrix.md). It minimizes squared Gram-matrix error, often called strain, rather than necessarily the sum of squared errors in raw distances. Negative [eigenvalues](../../../../../../eigenvalue.md) signal that the dissimilarities cannot be represented exactly by Euclidean coordinates; discarding them produces an approximation whose adequacy should be inspected.

In the upper-right sketch, the supplied distances come from four points in a rectangle, and the two-dimensional reconstruction recovers that shape. The overall translation, rotation and reflection of the configuration are not identifiable from distances. **Classical scaling reconstructs centered geometry from pairwise distances.** If the input distances are computed from centered multivariate observations, classical scaling and [principal component analysis](../../../../../../principal-component-analysis.md) give the same score configuration up to an orthogonal transformation: their matrices $ZZ^T$ and $Z^TZ$ share the nonzero squared singular values.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
