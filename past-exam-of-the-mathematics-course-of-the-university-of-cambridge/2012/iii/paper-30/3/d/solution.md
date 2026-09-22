<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use consistently wired boundary conditions in increasing finite boxes and let $\phi_{p,q}^{\mathrm w}$ be the usual wired infinite-volume [random-cluster measure](../../../../../../random-cluster-model.md). The finite-volume comparison just proved applies with boundary [graph vertices](../../../../../../vertex-graph-theory.md) identified, since it is still a comparison on a finite graph. Passing to the infinite-volume limit preserves the inequality for every [increasing event](../../../../../../increasing-event.md) determined by finitely many [edges](../../../../../../edge-of-a-graph.md).

For fixed $m$, let $A_m$ be the event that the origin connects by an [open path](../../../../../../open-path-in-bond-percolation.md) in $[-m,m]^2$ to its boundary. It is such a finite [increasing event](../../../../../../increasing-event.md). Therefore, for $q_1\le q_2$,

$$
\phi_{p,q_1}^{\mathrm w}(A_m)\ge\phi_{p,q_2}^{\mathrm w}(A_m).
$$

The events decrease to the event that the origin has an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md), by local finiteness. [Continuity from above of a measure](../../../../../../continuity-from-above-of-a-measure.md) gives

$$
\theta^{\mathrm w}(p,q_1)\ge\theta^{\mathrm w}(p,q_2).
$$

Define the [random-cluster critical probability](../../../../../../random-cluster-critical-probability.md) by $p_c(q)=\inf\{p:\theta^{\mathrm w}(p,q)>0\}$. The set in which percolation occurs at $q_2$ is a subset of that at $q_1$, whence

$$
\boxed{q_1\le q_2\quad\Longrightarrow\quad p_c(q_1)\le p_c(q_2).}
$$

The same proof works if free boundary conditions are used consistently throughout. It compares critical [probabilities](../../../../../../probability.md); it does not presume whether an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) exists at the critical parameter itself.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
