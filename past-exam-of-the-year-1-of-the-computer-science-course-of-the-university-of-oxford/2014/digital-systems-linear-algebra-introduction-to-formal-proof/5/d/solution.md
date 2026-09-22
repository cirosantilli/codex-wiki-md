<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [pivot columns](../../../../../pivot-column.md) of the [reduced row echelon form](../../../../../reduced-row-echelon-form.md) are columns 1 and 3. Take those columns of the original [matrix](../../../../../matrix.md), since [elementary row operations](../../../../../elementary-row-operation.md) need not preserve the original [column space](../../../../../column-space.md):

$$
\boxed{\left\{\begin{pmatrix}-1\\1\\2\end{pmatrix},\begin{pmatrix}3\\2\\5\end{pmatrix}\right\}.}
$$

For an explicit spanning check, column 2 is $-2a_1$, column 4 is $-a_1+2a_3$, and column 5 is $3a_1-2a_3$. The first two coordinates of the displayed columns form a $2\times2$ [matrix](../../../../../matrix.md) of [determinant](../../../../../determinant.md) $-5\ne0$, proving their [linear independence](../../../../../linear-independence.md). They are therefore a [basis](../../../../../basis.md) of the [column space](../../../../../column-space.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
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
