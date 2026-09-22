<h1 id="5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $B a=\sum_{j=1}^n a_jN_j$, and let $R f=(f(x_1),\ldots,f(x_n))^T$. We use the standard interpolation convention of distinct ordered sites $x_1<\cdots<x_n$. Together with $N_i(x_i)>0$, the [Schoenberg–Whitney theorem](../../../../../../schoenberg-whitney-theorem.md) makes the [B-spline collocation matrix](../../../../../../b-spline-collocation-matrix.md) $A$ invertible. Equivalently, its invertibility is implicit in the existence of the interpolation operator for every data vector.

If distinctness is not understood, the printed positivity condition alone is insufficient. For the order-two basis on [spline knots](../../../../../../spline-knot.md) $1,2,3,4$, take $x_1=x_2=5/2$. Both diagonal [B-spline](../../../../../../b-spline.md) values are $1/2>0$, but the two rows of $A$ coincide. Arbitrary data cannot then be interpolated uniquely. The norm statement below concerns the intended well-defined interpolation operator.

[Spline interpolation](../../../../../../spline-interpolation.md) determines the coefficient vector by $Aa=Rf$, and hence

$$
P_{\mathbf x}=B A^{-1}R.
$$

Nonnegativity and the [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) give

$$
\|Ba\|_\infty\le\|a\|_{\ell^\infty}.
$$

For completeness, extend the finite [spline knot sequence](../../../../../../spline-knot-sequence.md) beyond both ends. For the full sequence the order-one interval indicators sum to one. Summing the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) and shifting the index in its second term combines the two coefficients of each lower-order [B-spline](../../../../../../b-spline.md) to one, so induction gives partition of unity at every order. Our finite collection is a subset of that nonnegative collection, and thus has sum at most one. Repeated [spline knots](../../../../../../spline-knot.md) are handled by the standard zero-term convention or a knot limit. This argument controls the entire interval, not only the basic knot interval.

Since $\|Rf\|_{\ell^\infty}\le\|f\|_\infty$, the [operator norm](../../../../../../operator-norm.md) upper bound is

$$
\|P_{\mathbf x}f\|_\infty
\le\|A^{-1}\|_{\ell^\infty}\|f\|_\infty.
$$

Here the matrix [operator norm](../../../../../../operator-norm.md) is the maximum absolute row sum. For the lower bound, choose a row of $A^{-1}$ with maximum absolute row sum and a data vector $y$ whose components are the signs of that row's entries. Then $\|y\|_{\ell^\infty}=1$ and

$$
\|A^{-1}y\|_{\ell^\infty}=\|A^{-1}\|_{\ell^\infty}.
$$

A continuous piecewise-linear function taking these values at the distinct ordered sites, and constant outside their range, has [supremum norm](../../../../../../supremum-norm.md) one. Apply the given [uniform-norm stability of a B-spline basis](../../../../../../uniform-norm-stability-of-a-b-spline-basis.md) to its coefficient vector:

$$
\|P_{\mathbf x}f\|_\infty
=\|B A^{-1}y\|_\infty
\ge\frac1{d_k}\|A^{-1}y\|_{\ell^\infty}.
$$

Therefore

$$
\boxed{\frac1{d_k}\|A^{-1}\|_{\ell^\infty}
\le\|P_{\mathbf x}\|_{L^\infty}
\le\|A^{-1}\|_{\ell^\infty}}.
$$

The construction of the bounded continuous data extension is what permits the matrix norm to give a lower bound for a function-space [operator norm](../../../../../../operator-norm.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [5](../../5.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
