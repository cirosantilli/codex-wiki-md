<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the given [topological ordering](../../../../../../topological-ordering.md). Since $j$ precedes $k$, $j$ is not a descendant of $k$; since they are nonadjacent, it is not a parent of $k$. The [local Markov property of a directed acyclic graph](../../../../../../local-markov-property-of-a-directed-acyclic-graph.md) says that a node is d-separated from all its nondescendants other than its parents by its parent set. Therefore $j$ and $k$ are d-separated by $\operatorname{pa}(k)$.

It follows that adjacency of $Z_1,Z_2$ is certified by rejecting every null hypothesis

$$
Z_1\perp\!\!\!\perp Z_2\mid Z_S,
\qquad S\subseteq\{3,\ldots,p\}.
$$

If the vertices were nonadjacent, the theorem would supply one such separating parent set, whichever vertex comes later.

To certify that $X_1$ is a parent of $Y$, first reject

$$
X_1\perp\!\!\!\perp Y\mid (I,X_S)
$$

for every $S\subseteq\{2,\ldots,d\}$, which forces adjacency. Then reject

$$
I\perp\!\!\!\perp Y\mid X_S
$$

for every such $S$. If the adjacent edge were $Y\to X_1$, then $I\to X_1\leftarrow Y$ would orient $X_1$ as a collider, and the parent-set argument would provide a separator not containing $X_1$, contradicting the second collection of rejections. Hence the edge is $X_1\to Y$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
