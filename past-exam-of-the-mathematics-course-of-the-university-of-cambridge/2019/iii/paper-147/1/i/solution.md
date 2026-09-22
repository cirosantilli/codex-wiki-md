<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $x_1,x_2\in X$, let $d(x_1,x_2)$ be the number of vertices of $Y$ adjacent to both. The required number $Q$ of ordered quadruples is

$$
Q=\sum_{x_1,x_2\in X}d(x_1,x_2)^2.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) first gives

$$
Q\geq\frac1{|X|^2}\left(\sum_{x_1,x_2}d(x_1,x_2)\right)^2.
$$

Reverse the order of counting. A vertex $y\in Y$ contributes $\deg(y)^2$ ordered pairs, so a second application of Cauchy-Schwarz and the assumed [edge density of a bipartite graph](../../../../../../edge-density-of-a-bipartite-graph.md) give

$$
\sum_{x_1,x_2}d(x_1,x_2)
=\sum_{y\in Y}\deg(y)^2
\geq\frac1{|Y|}\left(\sum_y\deg(y)\right)^2
\geq\delta^2|X|^2|Y|.
$$

Therefore the [bipartite four-cycle count](../../../../../../bipartite-four-cycle-count.md) is

$$
\boxed{Q\geq\delta^4|X|^2|Y|^2.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 147](../../../paper-147-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
