<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $C=A\cup B$. Then

$$
\delta_\cup(\langle A\rangle,\langle B\rangle)
=\langle C^*\rangle-\langle C\rangle.
$$

Generate a uniformly random complete $(m-1)$-partite graph by independently assigning one of $m-1$ colours to each vertex and joining vertices of different colours. Such a graph contains the clique on $W$ exactly when the colouring is injective on $W$.

Construct $C^*$ by adjoining one forced set at a time. There are at most $n^l$ possible sets of size at most $l$. If $W$ is newly forced by $W_1,\ldots,W_r$, then, conditional on $W$ being rainbow, the events that each $W_i$ is not rainbow depend on disjoint petals $W_i\setminus W$. Since $l^2\leq m$, each has conditional probability at most $1/2$. Their simultaneous probability is therefore at most $2^{-r}$. A [union bound](../../../../../../boole-s-inequality.md) over the at most $n^l$ closure steps gives

$$
\mathbb P\!\left(
G\in\langle C^*\rangle-\langle C\rangle
\right)
\leq n^l2^{-r}.
$$

This is exactly the claimed proportion of complete $(m-1)$-partite graphs.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
