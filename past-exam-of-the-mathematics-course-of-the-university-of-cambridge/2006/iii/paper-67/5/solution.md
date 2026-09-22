<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

This addresses the general interpolation bound in part (I); the subsequent (a)–(c) address the cubic case in part (II). Write the interpolant in the [B-spline](../../../../../b-spline.md) [basis](../../../../../basis.md) as

$$
P_{\mathbf x}f=\sum_{j=1}^nc_jN_j,\qquad A_{\mathbf x}c=Rf,\qquad Rf=(f(x_1),\ldots,f(x_n))^T.
$$

The stipulated uniquely defined [spline interpolation operator](../../../../../spline-interpolation-operator.md) presupposes invertibility of the [B-spline collocation matrix](../../../../../b-spline-collocation-matrix.md). For the standard increasing distinct sites, the conditions $N_i(x_i)>0$ give it by the [Schoenberg–Whitney theorem](../../../../../schoenberg-whitney-theorem.md). Thus $c=A_{\mathbf x}^{-1}Rf$.

Use the standard partition-normalized [B-splines](../../../../../b-spline.md) of the question: they are nonnegative and satisfy the [subpartition of unity for B-splines](../../../../../subpartition-of-unity-for-b-splines.md), $\sum_jN_j(t)\leq1$. This also holds outside the basic knot interval; one may extend the knots and regard the finite family as a subfamily of a full partition of unity. The recurrence proof of the full partition is given in Question 6(c). Repeated knots retain the same nonnegativity and subpartition properties, with zero-denominator recurrence terms interpreted as zero or by knot limits. Consequently

$$
\left|\sum_jc_jN_j(t)\right|\leq\sum_j|c_j|N_j(t)\leq\|c\|_{\ell^\infty}.
$$

Sampling has [norm](../../../../../norm.md) at most one, $\|Rf\|_{\ell^\infty}\leq\|f\|_\infty$, and so

$$
\|P_{\mathbf x}f\|_\infty\leq\|A_{\mathbf x}^{-1}\|_{\ell^\infty}\|f\|_\infty,
\qquad\boxed{\|P_{\mathbf x}\|_{L^\infty}\leq\|A_{\mathbf x}^{-1}\|_{\ell^\infty}.}
$$

Here the induced [matrix](../../../../../matrix.md) [norm](../../../../../norm.md) is the maximum absolute row sum. The label $L^\infty$-normalized means the usual partition normalization, not rescaling each [spline](../../../../../spline-mathematics.md) to have maximum value one. Such a rescaling would invalidate the specific [coefficient](../../../../../coefficient.md) bound and the cardinal values used below.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
