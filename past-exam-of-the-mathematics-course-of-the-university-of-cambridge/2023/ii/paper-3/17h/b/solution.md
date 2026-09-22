<h1 id="17h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
P=v_0v_1\cdots v_\ell
$$

be a longest [path](../../../../../../path-in-a-graph.md) in $G$. Every neighbour of either endpoint lies on $P$. Suppose $\ell<2\delta(G)$. Among the $\ell$ possible cut positions of the path, the sets

$$
\{i:v_0v_i\in E(G)\},
\qquad
\{i:v_{i-1}v_\ell\in E(G)\}
$$

have total size greater than $\ell$, so they intersect. The corresponding two edges close a cycle containing all vertices of $P$.

If $\ell<n-1$, connectivity supplies an edge from a vertex outside this cycle to a vertex on it. Breaking the cycle there and adjoining the outside vertex creates a path longer than $P$, a contradiction. Hence

$$
\ell\geq\min(2\delta(G),n-1).
$$

Since $\delta(G)\geq t/2$ and $t\leq n-1$, the [long path from minimum degree](../../../../../../long-path-from-minimum-degree.md) gives $\ell\geq t$. Thus $G$ contains $P_t$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17H](../../17h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
