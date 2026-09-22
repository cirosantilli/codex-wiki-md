<h1 id="a/1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [topological space](../../../../../../topological-space.md) is [Lindelöf](../../../../../../lindelof-space.md) if every [open cover](../../../../../../open-cover.md) has a [countable](../../../../../../countable-set.md) subcover. We also prove the requested equivalence for [metrizable spaces](../../../../../../metrizable-space.md) here, after the two source definition leaves.

Choose a compatible [metric](../../../../../../metric.md) $d$. First suppose that $D$ is a [countable](../../../../../../countable-set.md) [dense subset](../../../../../../dense-set.md). The balls $B(d_0,q)$ with centers $d_0\in D$ and positive rational radii $q$ form a [countable](../../../../../../countable-set.md) [topological basis](../../../../../../basis-of-a-topology.md). Indeed, if $x\in U$ and $B(x,\epsilon)\subset U$, choose $d_0\in D$ with $d(x,d_0)<\epsilon/3$ and a rational $q$ between $d(x,d_0)$ and $\epsilon-d(x,d_0)$. The [triangle inequality](../../../../../../triangle-inequality.md) gives $x\in B(d_0,q)\subset U$.

For any [open cover](../../../../../../open-cover.md), retain the [topological basis](../../../../../../basis-of-a-topology.md) elements which are contained in some member of the cover, and choose one covering member for each such [topological basis](../../../../../../basis-of-a-topology.md) element. There are only countably many choices, and the resulting subfamily covers the [topological space](../../../../../../topological-space.md), since each point has a [topological basis](../../../../../../basis-of-a-topology.md) [neighborhood](../../../../../../neighbourhood-mathematics.md) inside a covering member. Thus a [separable](../../../../../../separable-topological-space.md) [metrizable space](../../../../../../metrizable-space.md) is [Lindelöf](../../../../../../lindelof-space.md).

Conversely, suppose the [metric space](../../../../../../metric-space.md) is [Lindelöf](../../../../../../lindelof-space.md). For each positive [integer](../../../../../../integer-split.md) $n$, the balls $B(x,1/n)$ cover it, so select a [countable](../../../../../../countable-set.md) subcover with centers in a [countable set](../../../../../../countable-set.md) $D_n$. The [union](../../../../../../set-union.md) $D=\bigcup_{n\ge1}D_n$ is [countable](../../../../../../countable-set.md) and [dense](../../../../../../dense-set.md): if $B(x,\epsilon)$ is a nonempty [open](../../../../../../open-set.md) ball, choose $n$ with $1/n<\epsilon$. One of the selected radius-$1/n$ balls contains $x$, so its center lies in $D\cap B(x,\epsilon)$. Therefore

$$
\boxed{\text{metrizable: separable}\quad\Longleftrightarrow\quad\text{Lindelöf}.}
$$

The [metric](../../../../../../metric.md) hypothesis is used in producing uniform small-ball covers and a [countable](../../../../../../countable-set.md) ball [topological basis](../../../../../../basis-of-a-topology.md); the equivalence need not hold for general [topological spaces](../../../../../../topological-space.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../../split.md)
7. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
