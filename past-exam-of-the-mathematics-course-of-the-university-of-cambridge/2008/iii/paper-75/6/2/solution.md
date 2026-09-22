<h1 id="6/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the standard nonnegative partition-normalized [B-splines](../../../../../../b-spline.md) $N_j$; their sum is at most one, and is exactly one for the complete clamped [basis](../../../../../../basis.md) on $[0,1]$. The printed question introduces $M_i$ only in its last [matrix](../../../../../../matrix.md) formula without defining it. The intended normalization is the [unit-integral normalization of a B-spline](../../../../../../unit-integral-normalization-of-a-b-spline.md):

$$
c_i=\int_0^1N_i(t)\,dt>0,\qquad M_i(t)=\frac{N_i(t)}{c_i},\qquad \int_0^1M_i(t)\,dt=1.
$$

For supports wholly inside the interval, $c_i=(t_{i+k}-t_i)/k$. The positivity and partition convention, sometimes called $L_\infty$ normalization, should not be confused with individually rescaling every [spline](../../../../../../spline-mathematics.md) to have maximum exactly one.

The characterization in part 1(a) gives the normal equations for the [orthogonal projection](../../../../../../orthogonal-projection.md):

$$
\left(f-\sum_ja_jN_j,N_i\right)_{L_2}=0,\qquad 1\le i\le n.
$$

Dividing each equation by $c_i$ yields

$$
Ga=d,\qquad G_{ij}=(M_i,N_j)_{L_2},\qquad d_i=(M_i,f)_{L_2}.
$$

This is the [mixed-normalization spline Gram matrix](../../../../../../mixed-normalization-spline-gram-matrix.md). It need not be symmetric, but $G=D^{-1}H$ with $D=\operatorname{diag}(c_i)$ and $H_{ij}=(N_i,N_j)_{L_2}$. The ordinary [Gram matrix](../../../../../../gram-matrix.md) $H$ is positive definite because the [splines](../../../../../../spline-mathematics.md) are linearly independent, so $G$ is invertible and $a=G^{-1}d$.

Since each $M_i$ is nonnegative and has integral one,

$$
|d_i|\le\int_0^1M_i(t)|f(t)|dt\le\|f\|_\infty,
\qquad\|d\|_{\ell_\infty}\le\|f\|_\infty.
$$

The induced [matrix](../../../../../../matrix.md) [operator norm](../../../../../../operator-norm.md) is the maximum absolute row sum, so

$$
\|a\|_{\ell_\infty}\le\|G^{-1}\|_{\ell_\infty\to\ell_\infty}\|f\|_\infty.
$$

Finally, nonnegativity and the [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) give

$$
|P_{\mathcal S}f(t)|
=\left|\sum_ja_jN_j(t)\right|
\le\|a\|_{\ell_\infty}\sum_jN_j(t)
\le\|a\|_{\ell_\infty}.
$$

Taking the supremum over $t$ and then over $\|f\|_\infty\le1$ proves the [maximum-norm bound for spline projection](../../../../../../maximum-norm-bound-for-spline-projection.md):

$$
\boxed{\|P_{\mathcal S}\|_\infty\le\|G^{-1}\|_{\ell_\infty\to\ell_\infty}.}
$$

The formulas also establish linearity and boundedness of the projection on continuous inputs. Its range is exactly the finite-dimensional [spline](../../../../../../spline-mathematics.md) space $\mathcal S$, since it fixes every [spline](../../../../../../spline-mathematics.md) in that space. Thus, when the [splines](../../../../../../spline-mathematics.md) are continuous, it is an operator $C[0,1]\to C[0,1]$ with range $\mathcal S$; it is not onto all of $C[0,1]$ as the printed wording says. For example, $e^t$ cannot belong to a fixed finite-degree [spline](../../../../../../spline-mathematics.md) space because it is not a [polynomial](../../../../../../polynomial-split.md) on any nonempty knot interval. The missing $M_i$ normalization and this range correction are needed for a precise reading of the result.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [6](../../6.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
