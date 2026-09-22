<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On a [tree](../../../../../../tree-graph-theory.md), every finite connected [induced subgraph](../../../../../../induced-subgraph.md) is itself a [tree](../../../../../../tree-graph-theory.md), and its only [spanning tree](../../../../../../spanning-tree.md) contains all its edges. Thus the [free uniform spanning forest](../../../../../../free-uniform-spanning-forest.md) is deterministic:

$$
\mathrm{FSF}=\delta_E.
$$

Suppose for a contradiction that $G$ is a [transient graph](../../../../../../transient-graph.md). By part (c), choose $e=\{a,b\}$ whose removal leaves two [transient graph](../../../../../../transient-graph.md) components $T_a,T_b$. Let $R_a,R_b<\infty$ be their [effective resistances to infinity](../../../../../../effective-resistance-to-infinity.md) measured from their respective endpoints.

In a wired finite exhaustion, the edge $e$ of resistance one is in parallel with the route from $a$ through $T_a$ to the wired boundary and back through $T_b$ to $b$. The latter route has resistance $R_{a,k}+R_{b,k}$, converging to $R_a+R_b$. Consequently the limiting wired [effective resistance](../../../../../../effective-resistance.md) is

$$
R_{\mathrm{eff}}^{\mathrm w}(a,b)=\frac{R_a+R_b}{1+R_a+R_b}<1.
$$

The [edge-inclusion formula for a uniform spanning tree](../../../../../../edge-inclusion-formula-for-a-uniform-spanning-tree.md), the one-edge case of the [transfer-current theorem](../../../../../../transfer-current-theorem.md), states that an edge of conductance $c_e$ is present with probability $c_eR_{\mathrm{eff}}(a,b)$. Passing to the wired limit and using $c_e=1$ gives

$$
\boxed{\mathbb P_{\mathrm{WSF}}(e\notin F)=\frac1{1+R_a+R_b}>0.}
$$

But under the [free uniform spanning forest](../../../../../../free-uniform-spanning-forest.md), $e$ is present with probability one. This contradicts $\mathrm{WSF}=\mathrm{FSF}$. Therefore **the tree is recurrent**. Combined with part (b), this characterizes equality of the free and wired [uniform spanning forests](../../../../../../uniform-spanning-forest.md) on locally finite unweighted [trees](../../../../../../tree-graph-theory.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
