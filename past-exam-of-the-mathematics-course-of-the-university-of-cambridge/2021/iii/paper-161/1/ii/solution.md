<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Regard each equation $P_i(x_j)=y_j$ as an incidence between the point $(x_j,y_j)$ and the graph of $P_i$. On each polynomial graph, join consecutive incident points by the intervening arc. If $I$ is the number of incidences, the resulting topological graph has

$$
M\geq I-m
$$

edges and $n$ vertices.

Two distinct degree-$d$ polynomial graphs meet in at most $d$ points because a nonzero polynomial of degree at most $d$ has at most $d$ real roots. Their drawn arcs therefore create at most $d$ genuine crossings. Parallel arcs with the same endpoints may be perturbed to cross once; for each pair of polynomials, such crossing-free lenses occur only between consecutive roots of their difference and hence at most $d$ times. The total number of genuine and added crossings is consequently

$$
O(dm^2).
$$

After these perturbations, a crossing-free subgraph is simple, so the sampling proof of the [Crossing lemma](../../../../../../crossing-lemma.md) applies to this topological graph.

If $M<6n$, then $I<m+6n$. Otherwise the crossing lemma gives

$$
c\frac{M^3}{n^2}\leq C_0dm^2,
$$

and hence

$$
M=O(d^{1/3}m^{2/3}n^{2/3}).
$$

Since $I\leq M+m$, both cases combine to prove the [incidences between points and polynomial graphs](../../../../../../incidences-between-points-and-polynomial-graphs.md) bound

$$
\boxed{I\leq C\left(m+n+d^{1/3}m^{2/3}n^{2/3}\right)}
$$

for an absolute constant $C$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
