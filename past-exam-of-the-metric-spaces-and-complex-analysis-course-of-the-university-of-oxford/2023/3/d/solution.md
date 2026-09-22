<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [d](../d.md)

The [identity theorem](../../../../identity-theorem.md) states: if $V\subseteq\mathbb C$ is a nonempty [connected](../../../../connected-space.md) [open set](../../../../open-set.md) and $p,q$ are [holomorphic functions](../../../../holomorphic-function-split.md) on $V$, and their equality set has a [limit point](../../../../limit-point.md) in $V$, then

$$
\boxed{p=q\quad\text{throughout }V}.
$$

The interior location of the [limit point](../../../../limit-point.md) and [connectedness](../../../../connected-space.md) are essential hypotheses.

For the proof put $h=p-q$. At any $z_0\in V$, its convergent [Taylor series](../../../../taylor-series.md) either has every coefficient zero, making $h$ zero on a neighbourhood, or has a first nonzero coefficient, of degree $m\geq0$. In the latter case,

$$
h(z)=(z-z_0)^m k(z),\qquad k(z_0)\ne0,
$$

where $k$ is [holomorphic](../../../../holomorphic-function-split.md) near $z_0$. By [continuity](../../../../continuous-function.md), $k$ is nonzero on a smaller disc. Thus any zero at $z_0$ is isolated unless $h$ vanishes on a neighbourhood. An accumulation of distinct zeros at the assumed interior [limit point](../../../../limit-point.md) therefore forces the neighbourhood alternative.

Let $E$ be the set of points of $V$ with a neighbourhood on which $h=0$. We have just proved $E\ne\varnothing$, and $E$ is an [open set](../../../../open-set.md). It is also a [closed set](../../../../closed-set.md) relative to $V$: a point of its [closure](../../../../closure-topology.md) outside $E$ would be approached by distinct points of $E$, hence by zeros, and the same [Taylor series](../../../../taylor-series.md) argument would place it in $E$. Since $V$ is [connected](../../../../connected-space.md), $E=V$. Thus $h=0$ on $V$, proving the theorem.

## ↑ Ancestors (12)

1. [d](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
