<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [elementary row operations](../../../../../elementary-row-operation.md) from bottom to top: $R_4\gets R_4-R_3$, $R_3\gets R_3-R_2$, and $R_2\gets R_2-R_1$. This order ensures that each subtraction uses the original preceding row. The result is the [upper triangular matrix](../../../../../upper-triangular-matrix.md)

$$
T=\begin{pmatrix}a&a&a&a\\0&b-a&b-a&b-a\\0&0&c-b&c-b\\0&0&0&d-c\end{pmatrix}.
$$

Put $\delta_1=a$, $\delta_2=b-a$, $\delta_3=c-b$, $\delta_4=d-c$. Row $i$ is either zero if $\delta_i=0$, or has its first nonzero entry in column $i$. Thus, for arbitrary real parameters, a [row echelon form](../../../../../row-echelon-form.md) is obtained by retaining the nonzero rows of $T$ in their existing order and moving every zero row to the bottom. This deals explicitly with vanishing parameters; an [upper triangular matrix](../../../../../upper-triangular-matrix.md) with an intermediate zero row is not yet a [row echelon form](../../../../../row-echelon-form.md).

The subtractions preserve the [determinant](../../../../../determinant.md), so the original [matrix](../../../../../matrix.md) has

$$
\det M=a(b-a)(c-b)(d-c).
$$

A square [matrix](../../../../../matrix.md) is invertible exactly when its [determinant](../../../../../determinant.md) is nonzero. Consequently,

$$
\boxed{M\text{ invertible}\iff a\ne0,\quad b\ne a,\quad c\ne b,\quad d\ne c.}
$$

These conditions concern consecutive parameters: no ordering, positivity, or pairwise distinctness of all four is required. More generally the [rank of a matrix](../../../../../matrix-rank.md) here is the number of nonzero $\delta_i$, because the retained nonzero rows have distinct leading columns.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
