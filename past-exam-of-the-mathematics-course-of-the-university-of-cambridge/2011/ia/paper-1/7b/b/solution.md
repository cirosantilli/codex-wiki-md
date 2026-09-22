<h1 id="7b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The equation is solvable exactly when $b\in\operatorname{im}A$, the [image of a linear map](../../../../../../image-of-a-linear-map.md), equivalently when the [rank of a matrix](../../../../../../matrix-rank.md) satisfies $\operatorname{rank}A=\operatorname{rank}[A\mid b]$. If it is solvable and $x_0$ is one solution, every solution is precisely

$$
x=x_0+v,\qquad v\in\ker A.
$$

Indeed differences of solutions lie in the [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md), and adding a kernel [vector](../../../../../../vector.md) preserves the equation. Hence **there are no solutions** when $b\notin\operatorname{im}A$; **one solution** when $A$ is invertible; and **infinitely many solutions** when $b\in\operatorname{im}A$ and $A$ is singular. In the last case the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) gives a nonzero kernel [vector](../../../../../../vector.md) $v$, and $x_0+tv$ gives distinct solutions for every real $t$. This proves that a finite number greater than one is impossible.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
