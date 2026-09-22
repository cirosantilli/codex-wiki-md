<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [cubic lattice](../../../../../../cubic-lattice.md) has [graph vertices](../../../../../../vertex-graph-theory.md) $\mathbb Z^d$ and an [edge](../../../../../../edge-of-a-graph.md) between $x,y$ when $\sum_i|x_i-y_i|=1$. In independent [site percolation](../../../../../../site-percolation-split.md), every [graph vertex](../../../../../../vertex-graph-theory.md) is open with [probability](../../../../../../probability.md) $p$ and closed with [probability](../../../../../../probability.md) $1-p$, independently. The open subgraph contains only open [graph vertices](../../../../../../vertex-graph-theory.md) and the [edges](../../../../../../edge-of-a-graph.md) between them. Let $C_p(0)$ be the open [connected component of a graph](../../../../../../component-graph-theory.md) containing $0$, with $C_p(0)=\varnothing$ when $0$ is closed. The [percolation probability](../../../../../../percolation-probability.md) is

$$
\boxed{\theta(p)=\mathbb P_p(|C_p(0)|=\infty)=\mathbb P_p(0\leftrightarrow\infty)}.
$$

Since the [cubic lattice](../../../../../../cubic-lattice.md) is a [locally finite graph](../../../../../../locally-finite-graph.md), the [König infinity lemma](../../../../../../konig-s-lemma.md) identifies an infinite open [connected component of a graph](../../../../../../component-graph-theory.md) with the existence of an infinite open [graph ray](../../../../../../ray-in-a-graph.md) from the origin. In particular, the origin itself must be open. The [percolation critical probability](../../../../../../percolation-critical-probability.md) is $p_c=\inf\{p:\theta(p)>0\}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
