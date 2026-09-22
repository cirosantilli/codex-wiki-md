<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the [spectral theorem](../../../../../../spectral-theorem.md), write $V=U\operatorname{diag}(v_1,\ldots,v_p)U^T$, where $U$ is [orthogonal](../../../../../../orthogonal-vectors.md) and each $v_j>0$. Choose the [whitening transformation](../../../../../../whitening-transformation.md)

$$
\boxed{L=V^{-1/2}=U\operatorname{diag}(v_1^{-1/2},\ldots,v_p^{-1/2})U^T.}
$$

A [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md) is [multivariate normal](../../../../../../multivariate-normal-distribution.md), and $LVL^T=I$. Thus $Z_i=L(Y_i-\mu)$ are independent $N_p(0,I)$ [random vectors](../../../../../../random-vector.md). Their whole joint distribution is independent of $\mu,V$.

Define $\bar Z=n^{-1}\sum_iZ_i$ and $S_Z=n^{-1}\sum_i(Z_i-\bar Z)(Z_i-\bar Z)^T$. These satisfy

$$
\bar Z=L(\bar Y-\mu),\qquad S_Z=LSL^T,
\qquad S_Z^{-1}=L^{-T}S^{-1}L^{-1}.
$$

Therefore

$$
\boxed{(\bar Y-\mu)^TS^{-1}(\bar Y-\mu)
=\bar Z^TS_Z^{-1}\bar Z.}
$$

The right side is a function of independent standard [multivariate normal](../../../../../../multivariate-normal-distribution.md) observations only, so its distribution depends on $n,p$ but not on $\mu,V$. This is the same [affine invariance of Hotelling's statistic](../../../../../../affine-invariance-of-hotelling-s-statistic.md) that permits multivariate mean tests with unknown [covariance](../../../../../../covariance.md). The proof concerns the jointly transformed mean and [covariance](../../../../../../covariance.md); whitening the mean alone would not establish the conclusion. Inverses exist almost surely under $n>p$. If $V$ is singular, no square [matrix](../../../../../../matrix.md) can whiten it to $I$, so nonsingularity of the population [covariance](../../../../../../covariance.md) is necessary as well.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
