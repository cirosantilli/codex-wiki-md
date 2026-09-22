<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [orthogonal projection](../../../../../../orthogonal-projection.md) has range $\mathcal S$, not all of $C[0,1]$: the latter is an [infinite-dimensional vector space](../../../../../../infinite-dimensional-vector-space.md) whereas $\mathcal S$ is a [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md). For a concrete counterexample, $e^x$ cannot belong to any finite-degree piecewise polynomial space, since all its [derivatives](../../../../../../derivative.md) are nonzero on every open interval. For $k\ge2$, the [B-splines](../../../../../../b-spline.md) are [continuous](../../../../../../continuous-function.md), so the [orthogonal projection](../../../../../../orthogonal-projection.md) is a map $C[0,1]\to\mathcal S\subset C[0,1]$. For order one it instead has a generally discontinuous piecewise constant range. For example, a single interval indicator on $[1/4,3/4)$ is the projection of the constant [function](../../../../../../function-split.md) one onto its span, and is not [continuous](../../../../../../continuous-function.md).

Write $s^*=\sum_ja_jN_j$. Since $M_i$ is a positive [scalar multiple](../../../../../../scalar-multiple.md) of $N_i$, the [operator normal equations](../../../../../../normal-equation-for-a-linear-inverse-problem.md) $\langle f-s^*,N_i\rangle=0$ are equivalent to

$$
Ga=b,\qquad b_i=\langle M_i,f\rangle.
$$

The [mixed-normalization spline Gram matrix](../../../../../../mixed-normalization-spline-gram-matrix.md) is invertible: $G=DH$ where $D_{ii}=k/(t_{i+k}-t_i)>0$ and $H_{ij}=\langle N_i,N_j\rangle$ is the ordinary [positive-definite matrix](../../../../../../positive-definite-matrix.md) of [inner products](../../../../../../inner-product.md) of a linearly independent [basis](../../../../../../basis.md). The positivity and [unit-integral normalization of a B-spline](../../../../../../unit-integral-normalization-of-a-b-spline.md) give $|b_i|\le\|f\|_\infty$. The [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) gives

$$
|s^*(t)|\le\|a\|_{\ell^\infty}\sum_jN_j(t)\le\|a\|_{\ell^\infty}.
$$

Here the [operator norm](../../../../../../operator-norm.md) of a [matrix](../../../../../../matrix.md) on $\ell^\infty$ is its maximum absolute row sum. Consequently,

$$
\|P_{\mathcal S}f\|_\infty\le\|a\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|b\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|f\|_\infty,
\qquad\boxed{\|P_{\mathcal S}\|_\infty\le\|G^{-1}\|_{\ell^\infty}.}
$$

This proves the [maximum-norm bound for spline projection](../../../../../../maximum-norm-bound-for-spline-projection.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
