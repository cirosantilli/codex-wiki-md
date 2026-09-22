<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Thomson principle](../../../../../../thomson-principle.md) states that the [effective resistance](../../../../../../effective-resistance.md) is the minimum [energy of a flow](../../../../../../energy-of-a-flow.md) among all [unit flows](../../../../../../unit-flow.md) from $a$ to $b$:

$$
R_{\mathrm{eff}}(a,b)=\min_{\operatorname{div}\vartheta=\mathbf1_a-\mathbf1_b}\sum_{e\in E}r_e\vartheta(e)^2.
$$

The [flow](../../../../../../flow.md) is antisymmetric on oriented edges, and the sum counts each unoriented edge once. The [Rayleigh monotonicity principle](../../../../../../rayleigh-monotonicity-principle.md) states that increasing edge resistances, including deleting edges by setting their resistance to infinity, cannot decrease the [effective resistance](../../../../../../effective-resistance.md). Decreasing resistances or identifying vertices cannot increase it.

Take a shortest [path in a graph](../../../../../../path-in-a-graph.md) from $a$ to $b$, of length $d=d_G(a,b)$, and send one unit of [flow](../../../../../../flow.md) along it, with zero [flow](../../../../../../flow.md) on all other edges. Its [energy of a flow](../../../../../../energy-of-a-flow.md) is $d$ because each edge resistance is one. The [Thomson principle](../../../../../../thomson-principle.md) gives

$$
\boxed{R_{\mathrm{eff}}(a,b)\leq d_G(a,b).}
$$

Alternatively, delete all edges outside that path and use the [Rayleigh monotonicity principle](../../../../../../rayleigh-monotonicity-principle.md); the remaining edges are in series, with total resistance $d$. When $a=b$, both quantities are zero.

## ↑ Ancestors (11)

1. [A](../a.md)
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
