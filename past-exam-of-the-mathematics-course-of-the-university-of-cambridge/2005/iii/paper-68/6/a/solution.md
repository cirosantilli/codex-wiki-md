<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For order $k\geq2$, set $g(u)=(u-t)_+^{k-2}$. Then $(u-t)g(u)=(u-t)_+^{k-1}$. Apply the given [divided difference](../../../../../../divided-difference.md) product identity with nodes $t_i,\ldots,t_{i+k}$ and multiply by the length $t_{i+k}-t_i$ of their knot interval:

$$
\begin{aligned}
N_{i,k}(t)
&=(t-t_i)[t_i,\ldots,t_{i+k-1}]g\\
&\quad +(t_{i+k}-t)[t_{i+1},\ldots,t_{i+k}]g.
\end{aligned}
$$

Using the definition of each lower-order normalized [B-spline](../../../../../../b-spline.md), the two [divided differences](../../../../../../divided-difference.md) are $N_{i,k-1}(t)/(t_{i+k-1}-t_i)$ and $N_{i+1,k-1}(t)/(t_{i+k}-t_{i+1})$. Hence the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) is

$$
\boxed{
N_{i,k}(t)=
\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)
+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t).}
$$

For completeness, the product identity itself follows from

$$
[t_0,\ldots,t_k](u-t)g(u)
=[t_0,\ldots,t_{k-1}]g+(t_k-t)[t_0,\ldots,t_k]g
$$

and the ordinary [divided difference](../../../../../../divided-difference.md) recurrence. Substitution yields the stated convex combination of the two order-$k-1$ [divided differences](../../../../../../divided-difference.md).

The initial order-one [splines](../../../../../../spline-mathematics.md) are the indicators $N_{i,1}(t)=\mathbf1_{[t_i,t_{i+1})}(t)$. For repeated knots, a term with zero knot-span denominator is defined as zero; this agrees with the standard limiting basis convention. The recurrence uses the [partition of unity](../../../../../../partition-of-unity.md) normalization with $0\leq N_{i,k}\leq1$, not a separate rescaling of each [spline](../../../../../../spline-mathematics.md) to make its actual supremum exactly one. The original PDF recurrence has the denominators above; several of these indices and signs were corrupted in the converted TeX.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
