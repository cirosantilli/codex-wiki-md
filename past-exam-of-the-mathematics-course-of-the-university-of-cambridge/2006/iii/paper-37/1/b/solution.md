<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $e=\{a,b\}$ be an [edge](../../../../../../edge-of-a-graph.md) of $G$. Apply the preceding result with source $a$ and sink $b$. A [tree](../../../../../../tree-graph-theory.md) contains $e$ exactly when its unique path from $a$ to $b$ is the single [edge](../../../../../../edge-of-a-graph.md) $e$, in the positive direction. Consequently the unit electrical current on $e$ is $\mathbb P(e\in T)$. By [Ohm's law](../../../../../../ohm-s-law.md) and the definition of [effective resistance](../../../../../../effective-resistance.md),

$$
\boxed{\mathbb P(e\in T)=R_{\mathrm{eff}}^G(a,b),}
$$

since this [edge](../../../../../../edge-of-a-graph.md) has unit resistance. This is the unit-conductance case of the [edge-inclusion formula for a uniform spanning tree](../../../../../../edge-inclusion-formula-for-a-uniform-spanning-tree.md).

The general principle needed is [Rayleigh monotonicity principle](../../../../../../rayleigh-monotonicity-principle.md): adding [edges](../../../../../../edge-of-a-graph.md), or decreasing their resistances, cannot increase the [effective resistance](../../../../../../effective-resistance.md) between fixed terminals. One precise variational formulation is the [Thomson principle](../../../../../../thomson-principle.md):

$$
R_{\mathrm{eff}}(a,b)=\min\left\{\sum_e r_ej_e^2:j\text{ is a unit flow from }a\text{ to }b\right\},
$$

with one orientation chosen for each unoriented [edge](../../../../../../edge-of-a-graph.md). To see this, write any [unit flow](../../../../../../unit-flow.md) as $i+k$, where $i$ is the electrical unit current and $k$ has zero divergence. Since $r_ei_e$ is a potential difference, summation by parts gives $\sum_er_ei_ek_e=0$. Thus its energy is $\sum_er_ei_e^2+\sum_er_ek_e^2$, minimized by $i$. The energy of $i$ equals its terminal voltage drop, hence the [effective resistance](../../../../../../effective-resistance.md).

Extend any [unit flow](../../../../../../unit-flow.md) on $G$ to $G'$ by zero on all new [edges](../../../../../../edge-of-a-graph.md). It is still a [unit flow](../../../../../../unit-flow.md), including at new [graph vertices](../../../../../../vertex-graph-theory.md), and its energy is unchanged. The variational minimum on $G'$ is therefore no larger. Using the edge-inclusion formula in both [graphs](../../../../../../graph-split.md) gives

$$
\boxed{\mathbb P(e\in T)\ge\mathbb P(e\in T').}
$$

The [graphs](../../../../../../graph-split.md) are understood to be finite and connected, as required for their uniform spanning-tree laws. The comparison allows added [graph vertices](../../../../../../vertex-graph-theory.md) as well as added [edges](../../../../../../edge-of-a-graph.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
