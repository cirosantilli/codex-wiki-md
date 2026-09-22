# Minimum-weight edge cover by matching savings

↑ **Parent:** [Maximum-weight matching](maximum-weight-matching.md)

For a finite [graph](graph-split.md) without an [isolated vertex](isolated-vertex.md) and with nonnegative edge weights, put $c_v=\min_{e\ni v}w(e)$ and let $e_v$ attain this minimum. Define savings $p(uv)=c_u+c_v-w(uv)$ and baseline $B=\sum_vc_v$. A [maximum-weight matching](maximum-weight-matching.md) $M$ with weights $p$, allowing arbitrary [cardinality](cardinality.md), gives a minimum-weight [edge cover](edge-cover.md)

$$
F_M=M\cup\{e_v:v\text{ is unmatched by }M\}.
$$

It replaces separate cheapest coverage of two endpoints by a shared [edge](edge-of-a-graph.md) when doing so saves enough weight. Savings can be negative even though original costs are nonnegative; such [edges](edge-of-a-graph.md) need not be selected.

**Proof.** The construction covers all [vertices](vertex-graph-theory.md). Duplicate selected [edges](edge-of-a-graph.md) are counted once, so nonnegative weights give $w(F_M)\leq B-p(M)$. Take an optimal [edge cover](edge-cover.md) and delete redundant [edges](edge-of-a-graph.md) to make it inclusion-minimal without increasing cost. Its components are [star graphs](star-graph-theory.md), by the argument for the [edge cover and matching identity](edge-cover-and-matching-identity.md). Select one [edge](edge-of-a-graph.md) from each component to obtain a [matching in a graph](matching-graph-theory-split.md) $N$. A component with center $a$, selected leaf $b$ and other leaves $L$ contributes $w(ab)+\sum_{v\in L}c_v$ to $B-p(N)$, at most its total edge weight since $c_v\leq w(av)$. Thus $B-p(N)\leq\operatorname{OPT}$. Maximizing $p$ gives

$$
\operatorname{OPT}\leq w(F_M)\leq B-p(M)\leq B-p(N)\leq\operatorname{OPT},
$$

which proves both the construction and the displayed identity, including zero-weight cases. One call to a general-[graph](graph-split.md) [maximum-weight matching](maximum-weight-matching.md) [polynomial-time algorithm](polynomial-time-algorithm.md) suffices, together with linear-time preprocessing. Choosing a [maximum cardinality matching](maximum-cardinality-matching.md) under these modified weights would impose an unnecessary constraint and can spoil the reduction.[max\_weight\_matching, maxcardinality=False, and Notes on polynomial running time](maximum-weight-matching-documentation-by-networkx.md)

## ↑ Ancestors (7)

1. [Maximum-weight matching](maximum-weight-matching.md)
2. [Matching (graph theory)](matching-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Edge cover](edge-cover.md)
- [Maximum-weight matching documentation by NetworkX](maximum-weight-matching-documentation-by-networkx.md)
- [Minimum-weight edge cover](minimum-weight-edge-cover.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/3/d/iii/solution.md)
