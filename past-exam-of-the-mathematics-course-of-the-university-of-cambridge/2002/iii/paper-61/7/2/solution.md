<h1 id="7/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the standard $L_\infty$-oriented partition normalization of [B-splines](../../../../../../b-spline.md), in contrast to the unit-integral normalization. Thus $N_i\ge0$ and $\sum_iN_i(t)\le1$ on $[0,1]$, with equality for a complete [basis](../../../../../../basis.md) on its basic knot interval. This terminology does not mean that each [basis](../../../../../../basis.md) function's maximum is exactly one; for example an order-three cardinal spline has maximum $3/4$. Assume the [basis](../../../../../../basis.md) has positive support on the integration interval and is continuous, as is needed for a projection taking values in $C[0,1]$.

Let

$$
H_{ij}=\int_0^1N_i(t)N_j(t)\,dt,\qquad d_i=\int_0^1N_i(t)\,dt>0,\qquad D=\operatorname{diag}(d_i).
$$

The ordinary [Gram matrix](../../../../../../gram-matrix.md) $H$ is positive definite by [linear independence](../../../../../../linear-independence.md). The appropriate row-normalized, or [mixed-normalization spline Gram matrix](../../../../../../mixed-normalization-spline-gram-matrix.md), is

$$
\boxed{G=D^{-1}H,\qquad G_{ij}=\int_0^1M_i(t)N_j(t)\,dt,\qquad M_i=N_i/d_i.}
$$

Here $M_i$ is a unit-integral nonnegative spline. Unlike $H$, $G$ need not be symmetric. If the full support lies inside the interval, $d_i=(t_{i+k}-t_i)/k$; otherwise use the actual interval integral rather than that full-support formula.

The [normal equations](../../../../../../normal-equation.md) for the $L_2$ [orthogonal projection](../../../../../../orthogonal-projection.md) $P_{\mathcal S}f=\sum_i a_iN_i$ say $Ha=c$, with $c_i=\int fN_i$. Divide each row by $d_i$ to obtain

$$
Ga=b,\qquad b_i=\int_0^1f(t)M_i(t)\,dt.
$$

Nonnegativity and unit integral give $|b_i|\le\|f\|_\infty$. The [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) then gives

$$
|P_{\mathcal S}f(t)|\le\sum_i|a_i|N_i(t)\le\|a\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|f\|_\infty.
$$

Taking the supremum over $t$ and then over nonzero $f$ proves the [uniform norm bound for B-spline orthogonal projection](../../../../../../uniform-norm-bound-for-b-spline-orthogonal-projection.md):

$$
\boxed{\|P_{\mathcal S}\|_{C[0,1]\to C[0,1]}\le\|G^{-1}\|_{\ell^\infty}.}
$$

The row normalization is essential; replacing $G$ with the ordinary [Gram matrix](../../../../../../gram-matrix.md) would not be the same asserted estimate. The operator is defined on $C[0,1]$ and maps into its finite-dimensional spline subspace, **onto $\mathcal S$, not onto all of $C[0,1]$** as one phrase in the PDF says. Its range follows both from the formula and from reproducing every $s\in\mathcal S$.

If “$L_\infty$-normalized” were instead read literally as individually peak-one splines, their sum can exceed one. The basis-dependent factor $K=\|\sum_iN_i\|_\infty$ must then be retained: $\|P_{\mathcal S}\|_\infty\le K\|(D^{-1}H)^{-1}\|_{\ell^\infty}$. Equivalently the displayed bound without an outside factor uses $G=K^{-1}D^{-1}H$. The standard partition-normalized convention has $K\le1$ and yields the sharper bound proved above.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [7](../../7.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
