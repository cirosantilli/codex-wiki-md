<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Yes. Let $(x^{(k)})_{k\geq1}$ be any [sequence](../../../../../sequence.md) in $A$, where $x^{(k)}=(x_m^{(k)})_{m\geq1}$. At coordinate $m$, the values lie in the [compact interval](../../../../../compact-interval.md) $[-1/m,1/m]$. By part (a)(ii) we can successively extract a [convergent subsequence](../../../../../convergent-subsequence.md) for coordinate one, a further one for coordinate two, and so on. Taking the diagonal indices gives a single subsequence $(x^{(k_j)})$ for which

$$
x_m^{(k_j)}\longrightarrow x_m\quad\text{for every fixed }m.
$$

The [closed interval](../../../../../closed-real-interval.md) bound passes to the limit, so $|x_m|\leq1/m$. Hence $x_m\to0$ and $x=(x_m)\in A$.

Coordinate convergence alone would not imply [supremum norm](../../../../../supremum-norm.md) convergence. Here the common tail bound supplies the missing estimate. Given $\epsilon>0$, choose $M$ with $2/(M+1)<\epsilon$. For $m>M$,

$$
|x_m^{(k_j)}-x_m|\leq2/m\leq2/(M+1)<\epsilon.
$$

For the finitely many $m\leq M$, coordinate convergence makes all differences less than $\epsilon$ once $j$ is large. Therefore $d(x^{(k_j)},x)<\epsilon$, and

$$
\boxed{A\text{ is sequentially compact in the supremum norm metric}}.
$$

This is an instance of [compactness from uniformly vanishing sequence tails](../../../../../compactness-from-uniformly-vanishing-sequence-tails.md). The common $1/m$ bound is exactly what the coordinate vectors in part (i) lack.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
