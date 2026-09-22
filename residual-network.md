# Residual network

↑ **Parent:** [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)

For a [feasible flow](feasible-flow.md) $f$, each original directed [edge](edge-of-a-graph.md) $u\to v$ supplies a forward [residual network](residual-network.md) [edge](edge-of-a-graph.md) of capacity $c_{uv}-f_{uv}$ and a backward one $v\to u$ of capacity $f_{uv}$; zero-capacity residual [edges](edge-of-a-graph.md) may be omitted. The forward [edge](edge-of-a-graph.md) permits an increase, while the backward [edge](edge-of-a-graph.md) permits cancellation of existing [flow](flow.md). In particular, backward residual capacity is the amount already sent, rather than unused original capacity. If both original orientations exist, keep their residual contributions separate, or add capacities for contributions with the same direction. An [augmenting path](augmenting-path.md) uses these permitted changes while preserving [flow conservation](flow-conservation.md) and the [capacity constraints](capacity-constraint.md).

To see why cancellation matters, give all five directed [edges](edge-of-a-graph.md) $s\to a$, $s\to b$, $a\to b$, $a\to t$, $b\to t$ unit [flow network edge capacities](flow-network-edge-capacity.md). Starting from zero [flow](flow.md), an [augmenting path](augmenting-path.md) $s\to a\to b\to t$ carrying $1$ yields

$$
(f_{sa},f_{sb},f_{ab},f_{at},f_{bt})=(1,0,1,0,1),\qquad |f|=1.
$$

The remaining unused original [edges](edge-of-a-graph.md) are $s\to b$ and $a\to t$, which do not form a source-to-sink [graph path](path-in-a-graph.md). However, the backward residual [edge](edge-of-a-graph.md) $b\to a$ has capacity $f_{ab}=1$. Consequently the [residual network](residual-network.md) contains the [augmenting path](augmenting-path.md) $s\to b\to a\to t$, with residual capacities $1,1,1$.

Augment by $1$: increase $f_{sb}$ and $f_{at}$ from $0$ to $1$, and decrease $f_{ab}$ from $1$ to $0$. The result is

$$
(f_{sa},f_{sb},f_{ab},f_{at},f_{bt})=(1,1,0,1,1),\qquad |f|=2.
$$

Now [flow conservation](flow-conservation.md) is $1=0+1$ at $a$ and $1+0=1$ at $b$. The final [flow](flow.md) sends one unit along each of $s\to a\to t$ and $s\to b\to t$. The [cut of a flow network](cut-of-a-flow-network.md) $S=\{s\}$ has [cut capacity](cut-capacity.md) $1+1=2$, proving this is a [maximum flow](maximum-flow-problem.md). Traversing $b\to a$ in the [residual network](residual-network.md) revised the earlier routing decision; it did not send actual traffic along a nonexistent original [edge](edge-of-a-graph.md).

<a id="image-backward-residual-capacity-reroutes-the-first-unit-of-flow"></a>
![](residual-flow-rerouting.png)

**[Figure 27](#image-backward-residual-capacity-reroutes-the-first-unit-of-flow). Backward residual capacity reroutes the first unit of flow**. Before: one unit follows s to a to b to t. Middle: the residual augmenting path s to b to a to t cancels flow on a to b. After: two units use the separate paths, and the middle original edge carries zero flow.

**Table of contents**

- [Residual maximum flow is the remaining optimality gap](residual-maximum-flow-is-the-remaining-optimality-gap.md)
- [Augmenting path](augmenting-path.md)
  - [Widest augmenting path](widest-augmenting-path.md)
    - [Geometric convergence of widest-path augmentation](geometric-convergence-of-widest-path-augmentation.md)
  - [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md)
    - [Integrality of the Ford-Fulkerson algorithm](integrality-of-the-ford-fulkerson-algorithm.md)

## ↑ Ancestors (7)

1. [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
2. [Flow network](flow-network.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (28)

- [Augmenting path](augmenting-path.md)
- [Capacitated flow optimality conditions](capacitated-flow-optimality-conditions.md)
- [Directed cycle](directed-cycle.md)
- [Flow network](flow-network.md)
- [Flow network edge capacity](flow-network-edge-capacity.md)
- [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/20d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-40/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/b/ii/solution.md)
- [Residual network](residual-network.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Widest augmenting path](widest-augmenting-path.md)
