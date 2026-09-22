<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [within-group and between-group scatter decomposition](../../../../../../within-group-and-between-group-scatter-decomposition.md) separates noise from group separation: $W$ measures variation about each group [sample mean](../../../../../../sample-mean.md), and $B$ measures separation of those [means](../../../../../../expected-value.md) about the overall [sample mean](../../../../../../sample-mean.md). In [linear discriminant analysis](../../../../../../linear-discriminant-analysis.md), seek a projection $a^Tx$ maximizing between-group relative to within-group variation,

$$
\frac{a^TBa}{a^TWa}.
$$

Normalize by $a^TWa=1$; a [Lagrange multiplier](../../../../../../lagrange-multiplier.md) calculation gives the [generalized eigenvalue problem](../../../../../../generalized-eigenvalue-problem.md) $Ba=\lambda Wa$. The leading [canonical discriminant directions](../../../../../../canonical-discriminant-directions.md) have the largest [eigenvalues](../../../../../../eigenvalue.md), and subsequent directions are orthogonal in the $W$ inner product. There are at most $\min(p,g-1)$ nonzero separating directions. Projecting observations onto these directions gives a low-dimensional display of group separation.

For classification, estimate the common [covariance matrix](../../../../../../covariance-matrix.md) by $S_p=W/(n-g)$ and use the [linear discriminant analysis](../../../../../../linear-discriminant-analysis.md) scores

$$
d_\nu(x)=x^TS_p^{-1}\bar x_\nu-\frac12\bar x_\nu^TS_p^{-1}\bar x_\nu+\log\pi_\nu,
$$

where $\pi_\nu$ are class prior probabilities. Assign to the largest score. **The same within-group scatter sets the noise scale, while between-group scatter selects the directions in which the group means separate most strongly.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
