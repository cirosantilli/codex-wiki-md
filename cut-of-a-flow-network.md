# Cut of a flow network

↑ **Parent:** [Flow network](flow-network-split.md)

A source-to-sink [cut of a flow network](cut-of-a-flow-network.md) is a [partition of a set](partition-of-a-set.md) $(S,V\setminus S)$ of the [vertex set](vertex-set.md) of a [flow network](flow-network-split.md), with $s\in S$ and $t\notin S$. Its [cut capacity](cut-capacity.md) sums the [flow network edge capacities](flow-network-edge-capacity.md) of [directed edges](directed-edge.md) leaving $S$.[Graph Theory by Reinhard Diestel; Diestel, Flows, §6.2, printed p. 158: source-side partition and cut capacity](graph-theory-by-reinhard-diestel/flows-author-hosted-chapter-preview.md)

The side $S$ may contain any selection of the other [vertices](vertex-graph-theory.md); its [induced subgraph](induced-subgraph.md) need not be a [connected graph](connected-graph.md). For the five-[edge](edge-of-a-graph.md) [flow network](flow-network-split.md) with [flow network edge capacities](flow-network-edge-capacity.md) $(c_{sa},c_{sb},c_{ab},c_{at},c_{bt})=(3,2,1,2,3)$, $S=\{s\}$ gives the [partition of a set](partition-of-a-set.md) $(\{s\},\{a,b,t\})$. Only $s\to a$ and $s\to b$ leave this side, so its [cut capacity](cut-capacity.md) is $3+2=5$. Choosing $S=\{s,b\}$ instead puts $a\to b$ across the boundary in the incoming direction: its [flow network edge capacity](flow-network-edge-capacity.md) is excluded.

<a id="image-forward-cut-capacity-bounds-net-flow-with-backward-flow-subtracted"></a>
![](network-flow-directed-cut-certificate.png)

**[Figure 1](#image-forward-cut-capacity-bounds-net-flow-with-backward-flow-subtracted). Forward cut capacity bounds net flow, with backward flow subtracted**.

The left panel pairs a [feasible flow](feasible-flow.md) of [flow value](strength-of-a-flow.md) $5$ with a [cut of a flow network](cut-of-a-flow-network.md) of [cut capacity](cut-capacity.md) $5$, proving that each is optimal. The right panel uses the same [feasible flow](feasible-flow.md) but a different [cut of a flow network](cut-of-a-flow-network.md): the outward [flow](flow.md) is $3+3=6$ and the backward [flow](flow.md) is $1$, giving net [flow](flow.md) $6-1=5$. That [cut capacity](cut-capacity.md) is $6$, so it supplies a valid but less sharp bound. The dashed boundary marks a [partition of a set](partition-of-a-set.md), rather than an additional [edge](edge-of-a-graph.md) or a proposed route.

**Table of contents**

- [Minimum cut](minimum-cut.md)
  - [Diagonal cut in a nearest-neighbour lattice flow](diagonal-cut-in-a-nearest-neighbour-lattice-flow.md)
- [Cut capacity](cut-capacity.md)

## ↑ Ancestors (6)

1. [Flow network](flow-network-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Cut capacity](cut-capacity.md)
- [Cut of a flow network](cut-of-a-flow-network.md)
- [Flow](flow.md)
- [Flow network edge capacity](flow-network-edge-capacity.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Measurable Hall theorem](measurable-hall-theorem.md)
- [Minimum cut](minimum-cut.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/a/solution.md)
- [Residual network](residual-network.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Uniform capacity perturbation of a flow network](uniform-capacity-perturbation-of-a-flow-network.md)
