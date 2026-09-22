<h1 id="17f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [extremal number](../../../../../../extremal-number.md) $\operatorname{ex}(n,H)$ is the maximum number of [edges](../../../../../../edge-of-a-graph.md) in an $n$-vertex [graph](../../../../../../graph-split.md) containing no [subgraph](../../../../../../subgraph.md) [isomorphic](../../../../../../graph-isomorphism.md) to $H$.

Let $G$ be [triangle-free](../../../../../../triangle-free-graph.md) with $e$ edges. For every edge $uv$, the [neighbourhoods](../../../../../../graph-neighbourhood.md) of $u$ and $v$ are disjoint apart from their endpoints, so  
$d(u)+d(v)\leq n$. Summing over edges and applying [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_vd(v)^2=\sum_{uv\in E}(d(u)+d(v))\leq ne,
$$

while

$$
\sum_vd(v)^2\geq\frac{(\sum_vd(v))^2}{n}
=\frac{4e^2}{n}.
$$

**Thus $e\leq n^2/4$, proving the required [Mantel theorem](../../../../../../mantel-theorem.md) bound.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17F](../../17f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
