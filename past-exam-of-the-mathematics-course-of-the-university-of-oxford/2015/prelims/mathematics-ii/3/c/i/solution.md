<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

All three examples below have positive [integer](../../../../../../../integer-split.md) [coefficients](../../../../../../../coefficient.md), so they work under either convention for whether $0\in\mathbb N$.

For $R=1$, take $\boxed{a_n=1}$. This is the [geometric series](../../../../../../../geometric-series.md): it converges for $|z|<1$, and its terms fail to tend to zero for $|z|\geq1$.

For $R=0$, take $\boxed{a_n=n!}$, using the [factorial](../../../../../../../factorial.md) and $0!=1$. For every fixed $z\ne0$, the [absolute values](../../../../../../../absolute-value.md) of successive terms have ratio $(n+1)|z|$. This eventually exceeds two, so the terms grow without bound and the [series](../../../../../../../series-mathematics.md) cannot converge. At $z=0$ it is finite, giving [radius of convergence](../../../../../../../radius-of-convergence.md) zero.

For $R=1/\sqrt2$, take

$$
\boxed{a_n=2^{\lfloor n/2\rfloor},}
$$

using the [floor function](../../../../../../../floor-function.md). The [coefficients](../../../../../../../coefficient.md) satisfy

$$
\frac{(\sqrt2)^n}{\sqrt2}\leq a_n\leq(\sqrt2)^n.
$$

The upper bound and the [comparison test for series](../../../../../../../comparison-test-for-series.md) give [absolute convergence](../../../../../../../absolute-convergence.md) when $\sqrt2|z|<1$. The lower bound prevents the terms tending to zero when $\sqrt2|z|\geq1$. Hence the [radius of convergence](../../../../../../../radius-of-convergence.md) is exactly $1/\sqrt2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
