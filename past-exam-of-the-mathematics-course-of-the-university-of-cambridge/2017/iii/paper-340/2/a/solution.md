<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix the ordering of the [orthonormal basis](../../../../../../orthonormal-basis.md) and write $c_m=\langle f,g_m\rangle$, taking indices from $1$. The [linear N-term approximation](../../../../../../linear-n-term-approximation.md) retains the first $N$ coefficients:

$$
\boxed{f_N^{\mathrm{lin}}=\sum_{m=1}^Nc_mg_m.}
$$

Its index set is independent of $f$, so the map is an [orthogonal projection](../../../../../../orthogonal-projection.md) and is [linear](../../../../../../linearity.md).

For the [nonlinear N-term approximation](../../../../../../best-n-term-approximation.md), let $\Lambda_N(f)$ be any set of $N$ indices with greatest $|c_m|$, resolving ties arbitrarily and padding with zero coefficients if necessary. Since $(c_m)\in\ell^2$, such a selection exists. Then

$$
\boxed{f_N^{\mathrm{nonlin}}=\sum_{m\in\Lambda_N(f)}c_mg_m,\qquad\|f-f_N^{\mathrm{nonlin}}\|^2=\sum_{m\notin\Lambda_N(f)}|c_m|^2.}
$$

The [Parseval identity](../../../../../../parseval-identity.md) shows that for any fixed index set the displayed coefficients minimize the [Hilbert space](../../../../../../hilbert-space-split.md) error. Choosing the largest squared magnitudes minimizes the omitted sum over every set of at most $N$ indices. This is the [best N-term approximation](../../../../../../best-n-term-approximation.md); dependence of the selected indices on $f$ makes the operation nonlinear.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
