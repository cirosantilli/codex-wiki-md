<h1 id="15h/solution">Solution</h1>

↑ **Parent:** [15H](../15h.md)

For a finite [bipartite graph](../../../../../bipartite-graph.md) with left vertex set $L$, [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) says that a [matching in a graph](../../../../../matching-graph-theory.md) covering $L$ exists exactly when $|N(S)|\geq|S|$ for every $S\subseteq L$. Necessity follows because distinct matched neighbors of $S$ lie in $N(S)$.

For sufficiency, induct on $|L|$, the empty case being immediate. If a nonempty proper subset $S$ has $|N(S)|=|S|$, apply the induction hypothesis to the [graph](../../../../../graph-split.md) on $S,N(S)$. For the remaining [graph](../../../../../graph-split.md), every $T\subseteq L\setminus S$ satisfies

$$
|N(T)\setminus N(S)|=|N(T\cup S)|-|N(S)|\geq|T|,
$$

so induction matches the remaining vertices too. If there is no such tight subset and $|L|>1$, every nonempty proper subset has at least one extra neighbor. Select an edge and remove its endpoints. Each subset of the remaining left vertices loses at most one neighbor, so it still satisfies the required condition; induction supplies the rest of the [matching in a graph](../../../../../matching-graph-theory.md). The case $|L|=1$ follows directly from the condition.

For a [doubly stochastic matrix](../../../../../doubly-stochastic-matrix.md) $A=(a_{ij})$, make a [bipartite graph](../../../../../bipartite-graph.md) joining row $i$ to column $j$ when $a_{ij}>0$. For a row subset $S$,

$$
|S|=\sum_{i\in S}\sum_{j\in N(S)}a_{ij}
\leq\sum_{j\in N(S)}\sum_i a_{ij}=|N(S)|.
$$

[Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) therefore gives a [perfect matching](../../../../../perfect-matching.md), or a [permutation](../../../../../permutation.md) $\sigma$, with $\boxed{a_{i,\sigma(i)}>0\text{ for every }i}$.

## ↑ Ancestors (10)

1. [15H](../15h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
