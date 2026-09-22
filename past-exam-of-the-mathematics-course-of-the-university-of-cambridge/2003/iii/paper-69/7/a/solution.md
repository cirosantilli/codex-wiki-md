<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [orthogonal projection](../../../../../../orthogonal-projection.md) condition is $(f-s^*,N_i)=0$ for all $i$. Since $M_i=kN_i/(t_{i+k}-t_i)$, it is equivalently

$$
Ga=b,\qquad G_{ij}=(M_i,N_j),\qquad b_i=(M_i,f).
$$

The [mixed-normalization spline Gram matrix](../../../../../../mixed-normalization-spline-gram-matrix.md) is invertible: $G=D^{-1}H$, where $D_{ii}=(t_{i+k}-t_i)/k>0$ and $H_{ij}=(N_i,N_j)$ is the positive-definite ordinary [Gram matrix](../../../../../../gram-matrix.md) of the [basis](../../../../../../basis.md). Nonnegativity and the [unit-integral normalization of a B-spline](../../../../../../unit-integral-normalization-of-a-b-spline.md) give $|b_i|\le\|f\|_\infty\int_0^1M_i=\|f\|_\infty$. The [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) gives, on all of $[0,1]$,

$$
|s^*(t)|\le\sum_j|a_j|N_j(t)\le\|a\|_{\ell^\infty}.
$$

Consequently

$$
\|P_Sf\|_\infty\le\|a\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|b\|_{\ell^\infty}\le\|G^{-1}\|_{\ell^\infty}\|f\|_\infty,
$$

so

$$
\boxed{\|P_S\|_\infty\le\|G^{-1}\|_{\ell^\infty}}.
$$

This is the [maximum-norm bound for spline projection](../../../../../../maximum-norm-bound-for-spline-projection.md). Using a subpartition matters when the basic knot interval is a proper subinterval of $[0,1]$. As in the paper's assertion that the image lies in $C[0,1]$, the [spline](../../../../../../spline-mathematics.md) space here must consist of [continuous functions](../../../../../../continuous-function.md); order-one step splines or full-multiplicity interior knots do not have that property.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
