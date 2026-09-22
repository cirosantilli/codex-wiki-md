# Maximum flow problem

↑ **Parent:** [Flow network](flow-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_flow_problem)

The [maximum flow problem](maximum-flow-problem.md) maximises the [strength of a flow](strength-of-a-flow.md) from a source to a sink subject to [flow conservation](flow-conservation.md) and [flow network edge capacities](flow-network-edge-capacity.md). For the nonnegative arc amounts used in [flow network](flow-network.md), its objective is net outflow from the source:

$$
|f|=\sum_{v:(s,v)\in E}f_{sv}-\sum_{u:(u,s)\in E}f_{us}
=\sum_{u:(u,t)\in E}f_{ut}-\sum_{v:(t,v)\in E}f_{tv}.
$$

The equality follows by summing [flow conservation](flow-conservation.md) over all internal [vertices](vertex-graph-theory.md). Incoming source [flow](flow.md) must be subtracted: merely circulating traffic through $s$ does not deliver more to $t$. The [max-flow min-cut theorem](max-flow-min-cut-theorem.md) identifies the optimum with the least [cut capacity](cut-capacity.md) of a [cut of a flow network](cut-of-a-flow-network.md). A [feasible flow](feasible-flow.md) and a [cut of a flow network](cut-of-a-flow-network.md) of equal value certify optimality without requiring a particular choice of [augmenting paths](augmenting-path.md).

For the five-[edge](edge-of-a-graph.md) [flow network](flow-network.md) with [flow network edge capacities](flow-network-edge-capacity.md) $(3,2,1,2,3)$, take

$$
(f_{sa},f_{sb},f_{ab},f_{at},f_{bt})=(3,2,1,2,3).
$$

Every [capacity constraint](capacity-constraint.md) holds with equality. [Flow conservation](flow-conservation.md) at $a$ is $3=1+2$, and at $b$ it is $2+1=3$. The [strength of a flow](strength-of-a-flow.md) is $|f|=3+2=5$, also $2+3=5$ entering $t$. This [flow](flow.md) consists of $2$ units on the [graph path](path-in-a-graph.md) $s\to a\to t$, $2$ on $s\to b\to t$, and $1$ on $s\to a\to b\to t$. The [cut of a flow network](cut-of-a-flow-network.md) with source side $\{s\}$ has [cut capacity](cut-capacity.md) $3+2=5$, so no [feasible flow](feasible-flow.md) can do better.

Even a seemingly poor first [augmenting path](augmenting-path.md) $s\to a\to b\to t$, carrying $1$, does not cause failure in this example. It leaves [residual network](residual-network.md) capacity $2$ along $s\to a\to t$ and $2$ along $s\to b\to t$. These two subsequent [augmenting paths](augmenting-path.md) yield values $1$, $3$, and $5$, and produce exactly the [flow](flow.md) above. Backward [residual network](residual-network.md) [edges](edge-of-a-graph.md) become essential in the unit-capacity example under [residual network](residual-network.md), where this same first choice blocks every unused forward route.

Discrete assignment is another reason to study [maximum flow](maximum-flow-problem.md). Put unit-capacity [edges](edge-of-a-graph.md) from $s$ to job [vertices](vertex-graph-theory.md), from each job to eligible worker [vertices](vertex-graph-theory.md), and from workers to $t$. An integral [flow](flow.md) selects a [matching in a graph](matching-graph-theory.md): each job and worker participates at most once, and the [strength of a flow](strength-of-a-flow.md) counts assigned jobs. The [integral max-flow theorem](integral-max-flow-theorem.md) therefore turns maximum cardinality assignment into [maximum flow](maximum-flow-problem.md). Minimizing assignment costs is the related [assignment problem](assignment-problem.md), modeled by [minimum-cost flow](minimum-cost-flow-problem.md).[Goemans, Network flows, assignment formulation](https://ocw.mit.edu/courses/6-854j-advanced-algorithms-fall-2008/4064d889e5033a9915327a777d12b592_notes_flow.pdf)

**Table of contents**

- [Sports elimination by maximum flow](sports-elimination-by-maximum-flow.md)
- [Treatment capacity as a sink arc](treatment-capacity-as-a-sink-arc.md)
- [Server connectivity under component failures](server-connectivity-under-component-failures.md)
- [Edmonds–Karp algorithm](edmonds-karp-algorithm.md)
- [Maximum flow with vertex capacities](maximum-flow-with-vertex-capacities.md)
  - [Vertex splitting](vertex-splitting.md)

## ↑ Ancestors (6)

1. [Flow network](flow-network.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Flow network](flow-network.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Maximum flow with vertex capacities](maximum-flow-with-vertex-capacities.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/a/solution.md)
