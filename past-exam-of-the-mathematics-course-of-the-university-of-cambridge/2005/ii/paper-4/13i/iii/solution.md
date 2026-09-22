<h1 id="13i/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Fisher information](../../../../../../fisher-information-matrix.md) is

$$
I(\beta)=\nu\sum_i\mu_i^2x_ix_i^T
=\nu\begin{pmatrix}a&b\\b&c\end{pmatrix}.
$$

Under standard interior, full-rank and large-sample regularity conditions, the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is asymptotically normal with mean $\beta$ and covariance

$$
I(\beta)^{-1}
=\frac1{\nu(ac-b^2)}\begin{pmatrix}c&-b\\-b&a\end{pmatrix}.
$$

Therefore

$$
\boxed{\widehat\beta_2\ \dot\sim\
N\!\left(\beta_2,\frac{a}{\nu(ac-b^2)}\right)}.
$$

The sums already depend on sample size; no extra factor $1/n$ should be inserted. The variance is estimable by substituting fitted means. If all $z_i$ are the same, $ac-b^2=0$ and the two coefficients are not separately identifiable.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [13I](../../13i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
