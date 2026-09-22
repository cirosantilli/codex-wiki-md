<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix an [edge](../../../../../../edge-of-a-graph.md) $e=\{u,v\}$ and orient it from $u$ to $v$. For each [spanning tree](../../../../../../spanning-tree.md) $T$, let $\gamma_T$ be its unique [graph path](../../../../../../path-in-a-graph.md) from $u$ to $v$. Assign a signed unit [graph path](../../../../../../path-in-a-graph.md) flow $j_T$ to oriented [edges](../../../../../../edge-of-a-graph.md): value $+1$ in the direction used by $\gamma_T$, value $-1$ on the reversed orientation, and zero otherwise. Define its mean

$$
J(x,y)=\mathbb E\,j_T(x,y).
$$

Each $j_T$ has net divergence one at $u$, minus one at $v$ and zero elsewhere, so $J$ is a [unit flow](../../../../../../unit-flow.md). The [mean spanning-tree path current](../../../../../../mean-spanning-tree-path-current.md) also satisfies the [Kirchhoff cycle law](../../../../../../kirchhoff-cycle-law.md). Although its verification is permitted to be omitted, a short counting argument makes it explicit. Let $\mathcal F_{uv}$ be the [two-component spanning forests](../../../../../../two-component-spanning-forest.md) separating $u$ and $v$, write $A_F$ for the component containing $u$, and let $N_T$ be the number of [spanning trees](../../../../../../spanning-tree.md). Deleting an [edge](../../../../../../edge-of-a-graph.md) used by the oriented [tree](../../../../../../tree-graph-theory.md) [graph path](../../../../../../path-in-a-graph.md) gives one such forest. Conversely adjoining an [edge](../../../../../../edge-of-a-graph.md) across its two components gives a unique [tree](../../../../../../tree-graph-theory.md) with that [edge](../../../../../../edge-of-a-graph.md) on its $u$-to-$v$ [graph path](../../../../../../path-in-a-graph.md). Consequently

$$
J(x,y)=\frac1{N_T}\sum_{F\in\mathcal F_{uv}}\bigl(\mathbf1_{A_F}(x)-\mathbf1_{A_F}(y)\bigr)=h(x)-h(y),\qquad h(x)=\frac1{N_T}\sum_{F\in\mathcal F_{uv}}\mathbf1_{A_F}(x).
$$

The gradient form proves the [Kirchhoff cycle law](../../../../../../kirchhoff-cycle-law.md) directly and is [Ohm's law](../../../../../../ohm-s-law.md) for unit [edge](../../../../../../edge-of-a-graph.md) resistance. The [Kirchhoff node law](../../../../../../kirchhoff-node-law.md) then gives $Lh=\delta_u-\delta_v$, and the electrical [unit flow](../../../../../../unit-flow.md) is unique: the difference between two such [voltages](../../../../../../voltage.md) is a [harmonic function on a graph](../../../../../../discrete-harmonic-function.md) and hence constant on the connected finite [graph](../../../../../../graph-split.md).

If $e\in T$, its single-edge route is the unique [tree](../../../../../../tree-graph-theory.md) [graph path](../../../../../../path-in-a-graph.md) from $u$ to $v$, so $j_T(u,v)=1$. If $e\notin T$, that [tree](../../../../../../tree-graph-theory.md) [graph path](../../../../../../path-in-a-graph.md) does not use $e$, so $j_T(u,v)=0$. Therefore

$$
J(u,v)=\mathbb P(e\in T).
$$

By [Ohm's law](../../../../../../ohm-s-law.md), $J(u,v)=h(u)-h(v)$; for a unit terminal current, this [voltage](../../../../../../voltage.md) difference is exactly the [effective resistance](../../../../../../effective-resistance.md) between the terminals. We have proved the requested [edge-inclusion formula for a uniform spanning tree](../../../../../../edge-inclusion-formula-for-a-uniform-spanning-tree.md):

$$
\boxed{\mathbb P(e\in T)=R_{\mathrm{eff}}(u,v).}
$$

Now use [linearity of expectation](../../../../../../linearity-of-expectation.md) and the fact that every [spanning tree](../../../../../../spanning-tree.md) has exactly $n-1$ [edges](../../../../../../edge-of-a-graph.md). This gives [Foster's theorem](../../../../../../foster-s-theorem.md):

$$
\boxed{\sum_{e\in E}R_{\mathrm{eff}}(e)=\sum_{e\in E}\mathbb P(e\in T)=\mathbb E|T|=n-1.}
$$

The sums here use unoriented [edges](../../../../../../edge-of-a-graph.md) exactly once. For unit conductance this is the displayed identity; with conductances $c_e$ the inclusion [probability](../../../../../../probability.md) and summand become $c_eR_{\mathrm{eff}}(e)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
