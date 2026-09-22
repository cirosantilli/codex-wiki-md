<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $y=(f(x_1),\ldots,f(x_n))^T$ and write the interpolating [spline](../../../../../../spline-mathematics.md) as $P_xf=\sum_{j=1}^nc_jN_j$. The interpolation equations are $A_xc=y$, so $c=A_x^{-1}y$. Since $P_x$ is defined as a unique interpolant for arbitrary data, its [B-spline collocation matrix](../../../../../../b-spline-collocation-matrix.md) is invertible. Ordered sites satisfying diagonal positivity ensure this by question 7. Positivity alone without admissible ordering does not: two equal sites in overlapping [basis](../../../../../../basis.md) [supports](../../../../../../support.md) could give two identical rows. The [norm](../../../../../../norm.md) argument below uses the existence of the operator stipulated here.

Standard partition-normalized [B-splines](../../../../../../b-spline.md) satisfy $N_j\ge0$ and $\sum_{j=1}^nN_j\le1$. The latter is a [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md): extending the knot sequence gives a full partition of unity, and discarding [basis](../../../../../../basis.md) functions cannot increase its sum. Hence

$$
|P_xf(t)|\le\sum_j|c_j|N_j(t)\le\|c\|_{\ell^\infty}
\le\|A_x^{-1}\|_{\ell^\infty}\|y\|_{\ell^\infty}
\le\|A_x^{-1}\|_{\ell^\infty}\|f\|_\infty.
$$

Taking the supremum over $t$ and then over unit-[norm](../../../../../../norm.md) $f$ gives the [B-spline interpolation operator norm](../../../../../../b-spline-interpolation-operator-norm.md) estimate

$$
\boxed{\|P_x\|_{L^\infty}\le\|A_x^{-1}\|_{\ell^\infty}.}
$$

Here the [matrix](../../../../../../matrix.md) [norm](../../../../../../norm.md) is the induced maximum-row-sum [norm](../../../../../../norm.md), not the maximum of its individual entries. The proof only needs nonnegative [basis](../../../../../../basis.md) functions, their sum at most one, and invertible interpolation.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [4](../../4.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
