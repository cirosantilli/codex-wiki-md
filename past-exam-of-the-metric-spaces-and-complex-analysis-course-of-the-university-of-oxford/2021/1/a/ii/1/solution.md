<h1 id="1/a/ii/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The answers, in the order [completeness](../../../../../../completeness.md), [sequential compactness](../../../../../../sequentially-compact-space.md), [connectedness](../../../../../../connected-space.md), and [path connectedness](../../../../../../path-connected-space.md), are

$$
\boxed{\text{yes, no, yes, yes}.}
$$

Define $F(0)=0$ and $F(x)=\sqrt{x}\sin(1/x)$ for $x>0$. The estimate $|F(x)|\leq\sqrt{x}$ proves [continuity](../../../../../../continuous-function.md) at zero by the [squeeze theorem](../../../../../../squeeze-theorem.md); elsewhere it follows from the usual [continuous functions](../../../../../../continuous-function.md). Thus $X$ is the [graph of a function](../../../../../../graph-of-a-function.md) $F$ on the [closed set](../../../../../../closed-set.md) $[0,\infty)$.

To check closedness directly, if $(x_n,F(x_n))\to(x,y)$ in the [Euclidean plane](../../../../../../euclidean-plane.md), then $x\geq0$ and [continuity](../../../../../../continuous-function.md) gives $y=F(x)$. Therefore $X$ is a [closed subset](../../../../../../closed-set.md) of the [complete metric space](../../../../../../complete-metric-space.md) $\mathbb R^2$, hence is a [complete metric space](../../../../../../complete-metric-space.md). The [sequence](../../../../../../sequence.md) $(n,F(n))$ has no [convergent subsequence](../../../../../../convergent-subsequence.md), since its first [Cartesian coordinates](../../../../../../cartesian-coordinate-system.md) tends to infinity, so [sequential compactness](../../../../../../sequentially-compact-space.md) fails.

For any two points $(u,F(u)),(v,F(v))$, the map

$$
\gamma(s)=\bigl((1-s)u+sv,F((1-s)u+sv)\bigr),\qquad 0\leq s\leq1,
$$

is a [continuous path](../../../../../../continuous-path.md) in $X$ joining them. Thus $X$ is [path-connected](../../../../../../path-connected-space.md), and consequently [connected](../../../../../../connected-space.md). The factor $\sqrt{x}$ is crucial: the oscillations shrink to the single point $(0,0)$.

## ↑ Ancestors (14)

1. [1](../1.md)
2. [ii](../../ii.md)
3. [a](../../../a.md)
4. [1](../../../../1.md)
5. [2021](../../../../../2021-split.md)
6. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../../split.md)
7. [Metric spaces and complex analysis course of the University of Oxford](../../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
