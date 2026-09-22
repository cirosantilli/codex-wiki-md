<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Form a [bipartite graph](../../../../../../bipartite-graph.md) with one vertex for each row and one for each column, putting an edge $ij$ exactly where $a_{ij}>0$. For a set $S$ of row vertices, let $N(S)$ be its neighbouring column vertices. Since $A$ is a [doubly stochastic matrix](../../../../../../doubly-stochastic-matrix.md),

$$
|S|=\sum_{i\in S}\sum_j a_{ij}=\sum_{j\in N(S)}\sum_{i\in S}a_{ij}\leq\sum_{j\in N(S)}\sum_i a_{ij}=|N(S)|.
$$

The [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md) therefore supplies a [perfect matching](../../../../../../perfect-matching.md). Its incidence entries define a [permutation matrix](../../../../../../permutation-matrix.md) $P$ supported on the positive entries of $A$, hence on the ones of $B$. Entrywise $P\leq B$, so

$$
\boxed{B=P+C,\qquad C=B-P\geq0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
