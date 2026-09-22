# Mean spanning-tree path current

↑ **Parent:** [Transfer-current theorem](transfer-current-theorem.md)

In a finite unweighted [connected graph](connected-graph.md), take distinct [graph vertices](vertex-graph-theory.md) $a\ne z$ and orient the unique [graph path](path-in-a-graph.md) from $a$ to $z$ in a [uniform spanning tree](uniform-spanning-tree.md) and assign signed unit current to its [edges](edge-of-a-graph.md). Its mean over [trees](tree-graph-theory.md) is the electrical [unit flow](unit-flow.md) from $a$ to $z$. The [Kirchhoff node law](kirchhoff-node-law.md) follows by averaging [graph path](path-in-a-graph.md) divergences. For the [graph cycle](cycle-in-a-graph.md) law, let $\mathcal F_{az}$ be the [two-component spanning forests](two-component-spanning-forest.md) separating the terminals and $A_F$ the component containing $a$. Deleting a tree-path [edge](edge-of-a-graph.md) and conversely adjoining an [edge](edge-of-a-graph.md) across a forest cut are inverse operations. Hence the mean signed current on an [edge](edge-of-a-graph.md) $u\to v$ is

$$
J(u,v)=\frac1{|\mathcal T(G)|}\sum_{F\in\mathcal F_{az}}\bigl(\mathbf1_{A_F}(u)-\mathbf1_{A_F}(v)\bigr).
$$

This is the gradient of $h(u)=|\mathcal T(G)|^{-1}\sum_F\mathbf1_{A_F}(u)$, proving the [graph cycle](cycle-in-a-graph.md) law. In particular $R_{\mathrm{eff}}(a,z)=|\mathcal F_{az}|/|\mathcal T(G)|$. For an oriented existing [edge](edge-of-a-graph.md) $e=(a,z)$, that [edge](edge-of-a-graph.md) is used by the [tree](tree-graph-theory.md) [graph path](path-in-a-graph.md) exactly when it belongs to the [tree](tree-graph-theory.md), and then has positive orientation. Thus its mean current is $\mathbb P(e\in T)$, giving the [edge-inclusion formula for a uniform spanning tree](edge-inclusion-formula-for-a-uniform-spanning-tree.md) by [Ohm's law](ohm-s-law.md).

## ↑ Ancestors (8)

1. [Transfer-current theorem](transfer-current-theorem.md)
2. [Uniform spanning tree](uniform-spanning-tree.md)
3. [Spanning tree](spanning-tree.md)
4. [Tree (graph theory)](tree-graph-theory.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/3/a/solution.md)
- [Two-component spanning forest](two-component-spanning-forest.md)
