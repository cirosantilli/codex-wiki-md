<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There are $n$ basis [splines](../../../../../../spline-mathematics.md) for the stated $n+k$ knots; the upper limit $k$ in the printed basis list is an indexing slip. Let

$$
A_{ij}=N_j(x_i^*),\qquad i,j=1,\ldots,n.
$$

The strictly increasing sites and $t_i<x_i^*<t_{i+k}$ give invertibility by the [Schoenberg–Whitney theorem](../../../../../../schoenberg-whitney-theorem.md). The needed additional [matrix](../../../../../../matrix.md) property is [total nonnegativity of B-spline collocation matrices](../../../../../../total-nonnegativity-of-b-spline-collocation-matrices.md): every ordered minor of $A$ is nonnegative.

Here is a structural justification of that sign property. [Knot insertion](../../../../../../knot-insertion.md) refines [spline](../../../../../../spline-mathematics.md) coefficients by rules of the form $b_j=\alpha_j a_j+(1-\alpha_j)a_{j-1}$, $0\leq\alpha_j\leq1$, with the usual unchanged coefficients before the insertion and shifted coefficients after it. Each coefficient map is a nonnegative rectangular bidiagonal [matrix](../../../../../../matrix.md); all its ordered minors are nonnegative, as its nonzero terms preserve row/column order. Products preserve this property by the [Cauchy–Binet formula](../../../../../../cauchy-binet-formula.md). Insert each ordered sampling site until it has full knot multiplicity. Evaluation at such a break is one of the refined coefficients, with a consistent one-sided convention. Consequently the [B-spline collocation matrix](../../../../../../b-spline-collocation-matrix.md) is an ordered row submatrix of the product of refinement [matrices](../../../../../../matrix.md), proving its nonnegative minors. This also applies to repeated admissible original knots.

Since $A$ is invertible and totally nonnegative, $\det A>0$. The [adjugate identity](../../../../../../adjugate-identity.md) gives the [checkerboard inverse of a totally nonnegative matrix](../../../../../../checkerboard-inverse-of-a-totally-nonnegative-matrix.md):

$$
(A^{-1})_{ij}=(-1)^{i+j}\frac{\det A_{\widehat j,\widehat i}}{\det A},
\qquad (-1)^{i+j}(A^{-1})_{ij}\geq0.
$$

Now for any [spline](../../../../../../spline-mathematics.md) $s=\sum_j a_jN_j$, its sampled-value vector is $y=Aa$. Hence the coefficient [linear functional](../../../../../../linear-functional.md) in the [dual basis](../../../../../../dual-basis.md) is exactly

$$
\boxed{\mu_i(s)=a_i=\sum_j(A^{-1})_{ij}s(x_j^*).}
$$

In particular $\mu_i(N_\ell)=\delta_{i\ell}$, verifying the hinted formula rather than assuming it. The [operator norm](../../../../../../operator-norm.md) of this [linear functional](../../../../../../linear-functional.md) is taken for the [uniform norm](../../../../../../supremum-norm.md) on the [spline](../../../../../../spline-mathematics.md)'s interval, containing all sampling sites. Evaluation at a sampling site has norm at most one, so

$$
|\mu_i(s)|\leq\left(\sum_j|(A^{-1})_{ij}|\right)\|s\|_\infty,
\qquad
\|\mu_i\|\leq\sum_j|(A^{-1})_{ij}|.
$$

For the given unit-norm alternating [spline](../../../../../../spline-mathematics.md), $s_*(x_j^*)=(-1)^j$, and the checkerboard signs make all terms in a fixed inverse row align:

$$
a_i^*=\mu_i(s_*)=\sum_j(A^{-1})_{ij}(-1)^j
=(-1)^i\sum_j|(A^{-1})_{ij}|.
$$

Since $\|s_*\|_\infty=1$, this supplies the reverse [operator norm](../../../../../../operator-norm.md) inequality and proves the [Chebyshev spline coefficient and dual norm equality](../../../../../../chebyshev-spline-coefficient-and-dual-norm-equality.md)

$$
\boxed{|a_i^*|=\|\mu_i\|=\sum_j|(A^{-1})_{ij}|,\qquad i=1,\ldots,n.}
$$

This [spline](../../../../../../spline-mathematics.md) attains the [operator norm](../../../../../../operator-norm.md) of each coefficient [linear functional](../../../../../../linear-functional.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
