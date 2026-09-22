<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $e_i$ be standard coordinate columns. The required [elementary matrix](../../../../../elementary-matrix.md) is

$$
\boxed{E=I_n+\alpha e_je_i^T,\qquad EA:\ R_j\gets R_j+\alpha R_i.}
$$

It is the [identity matrix](../../../../../identity-matrix.md) with the extra entry $\alpha$ in position $(j,i)$. Left [matrix multiplication](../../../../../matrix-multiplication.md) implements the row operation: all other rows are unchanged. Since $j>i$, $E$ is a lower [triangular matrix](../../../../../triangular-matrix.md) with every diagonal entry one. Part (a) therefore gives $\det(E)=1$ and

$$
\boxed{\det(EA)=\det(E)\det(A)=\det(A).}
$$

Hence adding a multiple of one row to another leaves the [determinant](../../../../../determinant.md) unchanged, even if $A$ is singular.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
