<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

The space of [polynomials](../../../../../polynomial-split.md) is not [complete](../../../../../completeness.md) for the [supremum norm](../../../../../supremum-norm.md) [metric](../../../../../metric.md) $d$. Consider

$$
p_n(t)=\sum_{k=0}^n(t/2)^k.
$$

The [geometric series](../../../../../geometric-series.md) has sum $F(t)=1/(1-t/2)$, and for $0\leq t\leq1$ its tail satisfies

$$
|F(t)-p_n(t)|=\frac{(t/2)^{n+1}}{1-t/2}\leq2^{-n}.
$$

Thus $(p_n)$ converges uniformly to $F$ and is a [Cauchy sequence](../../../../../cauchy-sequence.md) for $d$.

There is no [polynomial](../../../../../polynomial-split.md) $p$ agreeing with $F$ on $[0,1]$: otherwise the [polynomial](../../../../../polynomial-split.md) $(1-t/2)p(t)-1$ would vanish at infinitely many points and therefore be the zero [polynomial](../../../../../polynomial-split.md). Evaluating this identity at $t=2$ gives $-1=0$. By uniqueness of the [uniform limit](../../../../../uniform-limit.md), $(p_n)$ has no limit in $X$. This proves the claimed failure of [completeness](../../../../../completeness.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [c](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
