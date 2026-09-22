<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $N_{i,k}$ for the order-$k$ [B-spline](../../../../../../b-spline.md). At order one, $N_{i,1}=\mathbf1_{[t_i,t_{i+1})}$, and the finite sum is one on its basic knot interval. For larger order, the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) is

$$
N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t),
$$

with a zero-denominator term defined as zero. Sum over $i=1,\ldots,n$. For each interior lower-order index $j=2,\ldots,n$, the combined coefficient is

$$
\frac{t-t_j}{t_{j+k-1}-t_j}+\frac{t_{j+k-1}-t}{t_{j+k-1}-t_j}=1.
$$

The two unmatched lower-order terms have supports $[t_1,t_k]$ and $[t_{n+1},t_{n+k}]$, respectively, and vanish on the open basic interval $(t_k,t_{n+1})$. Induction therefore gives

$$
\boxed{\sum_{i=1}^nN_{i,k}(t)=1,\qquad t_k\le t\le t_{n+1}}.
$$

For simple knots and $k\ge2$, [continuity](../../../../../../continuous-function.md) extends the identity to both endpoints. In the order-one case and at admissible repeated endpoint knots, use the one-sided value from the basic interval. Extending the knot sequence in both directions also proves the [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md), $0\le\sum_iN_i\le1$ everywhere: the finite sum is a subset of a nonnegative full partition. That weaker global inequality will be needed in Question 7(a).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
