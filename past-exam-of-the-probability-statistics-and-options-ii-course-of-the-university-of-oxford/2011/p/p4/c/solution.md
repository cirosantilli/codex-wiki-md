<h1 id="p/p4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply part (b) to the first column of $A$, using an [orthogonal](../../../../../orthogonal-vectors.md) reflection to zero all entries below the first. Next apply a [Householder reflection](../../../../../householder-transformation.md) to the trailing subvector of the second column, embedded as $\operatorname{diag}(1,H_2)$ so it leaves the first row and the zeros already created intact. Continue similarly through the columns. If a trailing column subvector is zero, skip that step.

The product of these embedded [orthogonal](../../../../../orthogonal-vectors.md) matrices sends $A$ to an [upper triangular matrix](../../../../../upper-triangular-matrix.md) $R$. Write that product as $Q^T$; its transpose $Q$ is also [orthogonal](../../../../../orthogonal-vectors.md). Hence

$$
\boxed{Q^TA=R,\qquad A=QR.}
$$

The argument uses no inverse of $A$ and therefore includes singular matrices.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
