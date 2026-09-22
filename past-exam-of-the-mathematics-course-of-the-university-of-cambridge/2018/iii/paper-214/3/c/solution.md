<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $d=d_G(a,b)>0$, and for $i=1,\ldots,d$ put

$$
U_i=\{x:d_G(a,x)<i\},\qquad \Pi_i=\partial_eU_i.
$$

Each [edge cutset](../../../../../../edge-cutset.md) $\Pi_i$ separates $a$ from $b$. Adjacent vertices have [graph distances](../../../../../../distance-graph-theory.md) from $a$ differing by at most one. Hence an edge can cross at most one of these level boundaries, so the [edge cutsets](../../../../../../edge-cutset.md) are pairwise edge-disjoint. Write $k_i=|\Pi_i|\geq1$; then $\sum_i k_i\leq|E|$.

The [Nash-Williams inequality](../../../../../../nash-williams-inequality.md) for unit conductances gives

$$
R_{\mathrm{eff}}(a,b)\geq\sum_{i=1}^d\frac1{k_i}\geq\frac{d^2}{\sum_i k_i}\geq\frac{d^2}{|E|},
$$

where the middle inequality is the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). One can also derive the first inequality directly: every [unit flow](../../../../../../unit-flow.md) has signed net flux one through each $\Pi_i$, so its [energy of a flow](../../../../../../energy-of-a-flow.md) on that cut is at least $1/k_i$; sum over the disjoint cuts and use the [Thomson principle](../../../../../../thomson-principle.md).

Combining with the [commute time identity](../../../../../../commute-time-identity.md) yields

$$
\boxed{\mathbb E_a\tau_b+\mathbb E_b\tau_a=2|E|R_{\mathrm{eff}}(a,b)\geq2d_G(a,b)^2.}
$$

The case $a=b$ is trivial. A [path graph](../../../../../../path-graph.md), with $a,b$ its endpoints, attains equality.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
