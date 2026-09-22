<h1 id="e8/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For centred data, [classical multidimensional scaling](../../../../../../classical-multidimensional-scaling.md) from [Euclidean distances](../../../../../../euclidean-distance.md) constructs the observation [Gram matrix](../../../../../../gram-matrix.md)

$$
B=-\tfrac12HD^{(2)}H=XX^T,\qquad H=I-\tfrac1n\mathbf1\mathbf1^T,
$$

where $D^{(2)}_{ij}=\|x_i-x_j\|^2$. By part (i), its nonzero [eigenvalues](../../../../../../eigenvalue.md) agree with those of $X^TX$, the [matrix](../../../../../../matrix.md) used for [principal component analysis](../../../../../../principal-component-analysis.md) before dividing by a covariance normalization.

If $u_i=Xv_i/\sqrt{\lambda_i}$ is the unit observation-space [eigenvector](../../../../../../eigenvector.md), the corresponding [classical multidimensional scaling](../../../../../../classical-multidimensional-scaling.md) coordinate column is

$$
\boxed{\sqrt{\lambda_i}\,u_i=Xv_i}.
$$

That is exactly the column of [principal component scores](../../../../../../principal-component-score.md). Consequently **[classical multidimensional scaling](../../../../../../classical-multidimensional-scaling.md) of Euclidean pairwise distances recovers the same reduced coordinates as [principal component analysis](../../../../../../principal-component-analysis.md)**, up to signs and arbitrary [orthogonal transformations](../../../../../../orthogonal-transformation.md) within equal-[eigenvalue](../../../../../../eigenvalue.md) subspaces. Distances alone cannot fix translation or orientation. The equivalence presumes centred data and Euclidean distances; general dissimilarities need not yield a positive semidefinite [Gram matrix](../../../../../../gram-matrix.md) or a corresponding data [covariance matrix](../../../../../../covariance-matrix.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [E8](../../../e8.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../../split.md)
7. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
