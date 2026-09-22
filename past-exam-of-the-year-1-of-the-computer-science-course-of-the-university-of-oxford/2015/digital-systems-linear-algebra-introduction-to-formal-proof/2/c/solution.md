<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [pivot columns](../../../../../pivot-column.md) in the [row echelon form](../../../../../row-echelon-form.md) are columns 1 and 3. Use those columns of the **original** [matrix](../../../../../matrix.md) for a [basis](../../../../../basis.md) of the original [column space](../../../../../column-space.md):

$$
\boxed{\left\{\begin{pmatrix}1\\1\\-1\end{pmatrix},\begin{pmatrix}-1\\4\\6\end{pmatrix}\right\}.}
$$

For a direct spanning check, column 2 is twice column 1 and column 4 is $(17/5)$ times column 1 minus $(3/5)$ times column 3. The displayed columns are [linearly independent](../../../../../linear-independence.md), since the first two coordinates of $\alpha c_1+\beta c_3=0$ give $\alpha-\beta=0$ and $\alpha+4\beta=0$, so $\alpha=\beta=0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
