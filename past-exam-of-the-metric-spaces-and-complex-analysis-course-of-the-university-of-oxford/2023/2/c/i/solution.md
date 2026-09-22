<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

By the permitted [sequential compactness](../../../../../sequentially-compact-space.md) of the [product metric](../../../../../product-metric.md) space $X\times X$, the sequence of pairs $(\phi^{(k)}x,\phi^{(k)}y)$ has a [convergent subsequence](../../../../../convergent-subsequence.md), and hence a [Cauchy subsequence](../../../../../cauchy-subsequence.md). Choose two of its indices $r<s$ sufficiently late that

$$
d(\phi^{(r)}x,\phi^{(s)}x)+d(\phi^{(r)}y,\phi^{(s)}y)<\epsilon.
$$

The distance-increasing assumption iterates: $d(\phi^{(r)}u,\phi^{(r)}v)\geq d(u,v)$. With $n=s-r\geq1$, use $u=x,v=\phi^{(n)}x$, and then $u=y,v=\phi^{(n)}y$, to obtain

$$
d(x,\phi^{(n)}x)+d(y,\phi^{(n)}y)\leq d(\phi^{(r)}x,\phi^{(s)}x)+d(\phi^{(r)}y,\phi^{(s)}y)<\epsilon.
$$

Both summands are nonnegative, so

$$
\boxed{d(x,\phi^{(n)}x)<\epsilon,\qquad d(y,\phi^{(n)}y)<\epsilon}.
$$

The use of paired iterates ensures that the same positive return time works for both points.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [c](../../c.md)
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
