<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Horn copositive matrix](../../../../../../horn-copositive-matrix.md) is invariant under cyclic permutation of its five coordinates: its negative entries correspond precisely to neighboring indices on the five-cycle. For any $x\geq0$, cyclically relabel the coordinates so that $x_5$ is a smallest coordinate. In particular, $x_4-x_5\geq0$.

Using the stated identity in this coordinate order,

$$
x^THx=(x_1-x_2+x_3-x_4+x_5)^2+4x_2x_5+4x_1(x_4-x_5)\geq0.
$$

The square is nonnegative, and both remaining terms are nonnegative since $x_i\geq0$ and $x_4\geq x_5$. Cyclic invariance means the relabeling has not changed the [quadratic form](../../../../../../quadratic-form.md). Thus $H$ is a [copositive matrix](../../../../../../copositive-matrix.md) for every original ordering of $x$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
