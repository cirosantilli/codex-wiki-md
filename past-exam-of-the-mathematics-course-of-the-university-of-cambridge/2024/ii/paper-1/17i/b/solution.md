<h1 id="17i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $P=v_0\ldots v_\ell$ be a longest path. All neighbours of $v_0$ lie on $P$, in the colour class opposite to $v_0$, so $\ell\geq2k-1$. If $\ell\geq2k$, the first $2k$ edges give the required path. Otherwise $\ell=2k-1$, and all $k$ vertices of the opposite colour on $P$ must be neighbours of $v_0$; in particular $v_0v_\ell$ is an edge, giving a cycle of length $2k$. The graph $K_{k,k}$ has minimum degree $k$ but only $2k$ vertices, so it has no path of length $2k$.

For the stronger assertion, assume there is no $4$-cycle. Rotate a longest path about each edge from $v_0$ to obtain $k$ possible endpoints in the colour class of $v_0$. Every neighbour of each rotated endpoint lies on $P$, since otherwise the corresponding path could be extended. In a $4$-cycle-free bipartite graph, two vertices in one colour class have at most one common neighbour. The [neighbourhood bound for a square-free bipartite graph](../../../../../../neighbourhood-bound-for-a-square-free-bipartite-graph.md) therefore shows that the colour class opposite to $v_0$ contains at least $2k-1$ vertices of $P$. If the endpoints have opposite colours, repeating the argument from $v_\ell$ gives the same bound for the other class. If they have the same colour, their class has one more vertex on $P$ than the opposite class. In either case $P$ has at least $4k-2$ vertices and length at least $4k-3$. Consequently $G$ contains either such a path or a $4$-cycle.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17I](../../17i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
