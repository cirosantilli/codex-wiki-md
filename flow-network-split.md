# Flow network

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flow_network)

A [flow network](flow-network-split.md) is a [directed graph](directed-graph.md) $G=(V,E)$ with distinct source and sink [vertices](vertex-graph-theory.md) $s,t$ and a nonnegative [flow network edge capacity](flow-network-edge-capacity.md) $c_{uv}$ on each directed [edge](edge-of-a-graph.md) $(u,v)$. In the finite setting here, every [flow network edge capacity](flow-network-edge-capacity.md) is a finite real number. A [feasible flow](feasible-flow.md) assigns a nonnegative amount $f_{uv}$ to each original directed [edge](edge-of-a-graph.md), satisfies the [capacity constraints](capacity-constraint.md), and obeys [flow conservation](flow-conservation.md) at every other [vertex](vertex-graph-theory.md):

$$
0\leq f_{uv}\leq c_{uv},\qquad
\sum_{u:(u,v)\in E}f_{uv}=\sum_{w:(v,w)\in E}f_{vw}\quad(v\notin\{s,t\}).
$$

These are nonnegative arc amounts. The antisymmetric convention in [flow](flow.md) instead records net amounts $\theta_{uv}=f_{uv}-f_{vu}$, taking a missing arc amount as zero. The two conventions express the same [flow conservation](flow-conservation.md); keeping them distinct makes backward [residual network](residual-network.md) [edges](edge-of-a-graph.md) easier to interpret.

Think of [vertices](vertex-graph-theory.md) as routers, directed [edges](edge-of-a-graph.md) as communication links, [flow network edge capacities](flow-network-edge-capacity.md) as available bandwidth, and [flow](flow.md) as a steady transmission rate. An intermediate router can distribute incoming traffic among outgoing links, but [flow conservation](flow-conservation.md) prevents it from creating traffic. The [maximum flow problem](maximum-flow-problem.md) asks how much total traffic can pass from $s$ to $t$, allowing several [graph paths](path-in-a-graph.md) to share the work. The same [flow network](flow-network-split.md) language models transportation and abstract resource allocation.[Goemans, Network flows, introduction and maximum flow formulation](https://ocw.mit.edu/courses/6-854j-advanced-algorithms-fall-2008/4064d889e5033a9915327a777d12b592_notes_flow.pdf)

Our running [flow network](flow-network-split.md) has [vertices](vertex-graph-theory.md) $V=\{s,a,b,t\}$ and exactly five directed [edges](edge-of-a-graph.md), with [flow network edge capacities](flow-network-edge-capacity.md)

$$
(c_{sa},c_{sb},c_{ab},c_{at},c_{bt})=(3,2,1,2,3).
$$

The cross [edge](edge-of-a-graph.md) $a\to b$ lets traffic entering $a$ use spare capacity on $b\to t$. With this [edge](edge-of-a-graph.md) removed, the two separate [graph paths](path-in-a-graph.md) can carry only $\min(3,2)+\min(2,3)=4$; including it will let the [maximum flow](maximum-flow-problem.md) reach $5$. Thus a link's usefulness depends on the rest of the [flow network](flow-network-split.md), rather than just its own [flow network edge capacity](flow-network-edge-capacity.md).

**Table of contents**

- [Circulation in a flow network](circulation-in-a-flow-network.md)
- [Vertex capacity](vertex-capacity.md)
- [Maximum flow problem](maximum-flow-problem.md)
  - [Dinic's algorithm](dinic-s-algorithm.md)
  - [Sports elimination by maximum flow](sports-elimination-by-maximum-flow.md)
  - [Treatment capacity as a sink arc](treatment-capacity-as-a-sink-arc.md)
  - [Server connectivity under component failures](server-connectivity-under-component-failures.md)
  - [Edmonds–Karp algorithm](edmonds-karp-algorithm.md)
  - [Maximum flow with vertex capacities](maximum-flow-with-vertex-capacities.md)
    - [Vertex splitting](vertex-splitting.md)
- [Flow network edge capacity](flow-network-edge-capacity.md)
- [Capacity constraint](capacity-constraint.md)
- [Cut of a flow network](cut-of-a-flow-network.md)
  - [Minimum cut](minimum-cut.md)
    - [Diagonal cut in a nearest-neighbour lattice flow](diagonal-cut-in-a-nearest-neighbour-lattice-flow.md)
  - [Cut capacity](cut-capacity.md)
- [Flow](flow.md)
  - [Unit flow](unit-flow.md)
  - [Divergence of a flow](divergence-of-a-flow.md)
    - [Flow conservation](flow-conservation.md)
  - [Strength of a flow](strength-of-a-flow.md)
  - [Energy of a flow](energy-of-a-flow.md)
    - [Finite-energy flow criterion for transience](finite-energy-flow-criterion-for-transience.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
  - [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
  - [Uniform capacity perturbation of a flow network](uniform-capacity-perturbation-of-a-flow-network.md)
  - [Integral max-flow theorem](integral-max-flow-theorem.md)
  - [Kőnig's theorem (graph theory)](konig-s-theorem-graph-theory.md)
  - [Residual network](residual-network.md)
    - [Residual maximum flow is the remaining optimality gap](residual-maximum-flow-is-the-remaining-optimality-gap.md)
    - [Augmenting path](augmenting-path.md)
      - [Widest augmenting path](widest-augmenting-path.md)
        - [Geometric convergence of widest-path augmentation](geometric-convergence-of-widest-path-augmentation.md)
      - [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md)
        - [Integrality of the Ford-Fulkerson algorithm](integrality-of-the-ford-fulkerson-algorithm.md)
  - [Parametric maximum flow with one source capacity](parametric-maximum-flow-with-one-source-capacity.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Braess's paradox](braess-s-paradox.md)
- [Cut capacity](cut-capacity.md)
- [Cut of a flow network](cut-of-a-flow-network.md)
- [Divergence of a flow](divergence-of-a-flow.md)
- [Flow](flow.md)
- [Flow network](flow-network-split.md)
- [Fluid flow](fluid-flow.md)
- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Nonatomic congestion game](nonatomic-congestion-game.md)
- [Outdegree orientation criterion](outdegree-orientation-criterion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/a/solution.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Treatment capacity as a sink arc](treatment-capacity-as-a-sink-arc.md)
- [Uniform capacity perturbation of a flow network](uniform-capacity-perturbation-of-a-flow-network.md)
- [Vertex splitting](vertex-splitting.md)
