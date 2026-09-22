<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Rado's theorem](../../../../../../rado-s-theorem.md) states that a rational matrix is [partition regular](../../../../../../partition-regular-matrix.md) if and only if it has the [columns property](../../../../../../columns-property.md). By hypothesis each $A_i$ is partition regular, so choose a columns partition for each one. Form the block-diagonal matrix

$$
B=\operatorname{diag}(A_1,\ldots,A_n).
$$

Taking at stage $j$ the union of the $j$th blocks from the individual partitions, with empty blocks added after a partition ends, gives the columns property for $B$: each row block sees exactly the corresponding dependence for its $A_i$. Hence $B$ is partition regular by [Rado's theorem](../../../../../../rado-s-theorem.md). A monochromatic vector

$$
x=(x_1,\ldots,x_n)
$$

in the [kernel](../../../../../../kernel-of-a-linear-map.md) of $B$ satisfies $A_ix_i=0$ for every $i$, and all entries of all the $x_i$ have the same color.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
