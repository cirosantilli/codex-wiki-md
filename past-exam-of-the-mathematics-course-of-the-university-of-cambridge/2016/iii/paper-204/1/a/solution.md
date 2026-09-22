<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [bond percolation](../../../../../../bond-percolation-split.md) on an [undirected graph](../../../../../../undirected-graph.md) $G=(V,E)$, a configuration is $\omega\in\{0,1\}^E$. The [edge](../../../../../../edge-of-a-graph.md) $e$ is open when $\omega_e=1$ and closed when $\omega_e=0$. Under $\mathbb P_p$, the coordinates are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) of parameter $p$. For a countable [edge](../../../../../../edge-of-a-graph.md) set, use the [product sigma-algebra](../../../../../../product-sigma-algebra.md) and the [product measure](../../../../../../product-measure.md)

$$
\mathbb P_p=\bigotimes_{e\in E}\operatorname{Bernoulli}(p).
$$

The open [edges](../../../../../../edge-of-a-graph.md) form a random subgraph with the original [graph vertices](../../../../../../vertex-graph-theory.md). Its [connected components of a graph](../../../../../../component-graph-theory.md) are the [percolation clusters](../../../../../../percolation-cluster.md). Write $x\leftrightarrow y$ when an open [graph path](../../../../../../path-in-a-graph.md) joins $x$ to $y$; a zero-length [graph path](../../../../../../path-in-a-graph.md) is allowed, so $x\leftrightarrow x$ always holds. **The randomness is in the independently open bonds; all vertices remain present.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
