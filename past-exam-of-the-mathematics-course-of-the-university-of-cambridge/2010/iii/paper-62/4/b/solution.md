<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $s_j=t_{i+j}$ again and take $k\ge2$. Set $g(s)=(s-t)_+^{k-2}$, so $(s-t)g(s)=(s-t)_+^{k-1}$. Let

$$
H=[s_0,\ldots,s_{k-1}]g,\qquad K=[s_1,\ldots,s_k]g,\qquad G=[s_0,\ldots,s_k]g=\frac{K-H}{s_k-s_0}.
$$

The [Leibniz rule for divided differences](../../../../../../leibniz-rule-for-divided-differences.md), applied to the linear factor $s-t$, reads

$$
[s_0,\ldots,s_k]\bigl((s-t)g(s)\bigr)=(s_0-t)G+K.
$$

Multiply by $s_k-s_0$ and substitute $G$ to get $(t-s_0)H+(s_k-t)K$. Converting $H$ and $K$ to the lower-order normalized [B-splines](../../../../../../b-spline.md) proves the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md):

$$
\boxed{N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t).}
$$

It starts with $N_{i,1}=1_{[t_i,t_{i+1})}$. The coefficients are nonnegative wherever the corresponding lower-order [B-spline](../../../../../../b-spline.md) is nonzero, so induction proves nonnegativity.

For later use, extend the finite knot sequence to a strictly increasing sequence in both directions. The full order-one sum is one. When the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) is summed, the two coefficients of each fixed lower-order [B-spline](../../../../../../b-spline.md) add to one. Induction therefore gives a full partition of unity. Removing terms proves the [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md), $\sum_{i=1}^nN_{i,k}(t)\le1$. For repeated knots, the same statement follows by a limit of strictly increasing knot sequences, with the usual convention that a recurrence term with zero denominator is zero; the bound holds on each open knot interval and for the standard one-sided endpoint values. The terminology “$L_\infty$-normalized” refers to this standard basis normalization; it does not claim that each individual [B-spline](../../../../../../b-spline.md) has [supremum norm](../../../../../../supremum-norm.md) exactly one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
