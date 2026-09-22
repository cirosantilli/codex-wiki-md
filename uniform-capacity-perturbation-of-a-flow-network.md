# Uniform capacity perturbation of a flow network

↑ **Parent:** [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)

If every directed edge capacity increases by $\varepsilon$, a [cut of a flow network](cut-of-a-flow-network.md) with $m(S)$ outgoing edges gains $\varepsilon m(S)$. By the [max-flow min-cut theorem](max-flow-min-cut-theorem.md), the new [maximum flow](maximum-flow-problem.md) value is

$$
v(\varepsilon)=\min_{S:s\in S,\,t\notin S}\bigl(c(S)+\varepsilon m(S)\bigr).
$$

For a finite [flow network](flow-network.md), this is a nondecreasing concave piecewise-linear function, and its active cut can change as $\varepsilon$ varies. Two unit-capacity edge-disjoint two-edge source-to-sink paths gain $2\varepsilon$, refuting an invariably exact $\varepsilon$ increase. If there is a directed source-to-sink path, every cut has at least one outgoing edge and the increase is at least $\varepsilon$; without a path it can be zero.

## ↑ Ancestors (7)

1. [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
2. [Flow network](flow-network.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/d/solution.md)
