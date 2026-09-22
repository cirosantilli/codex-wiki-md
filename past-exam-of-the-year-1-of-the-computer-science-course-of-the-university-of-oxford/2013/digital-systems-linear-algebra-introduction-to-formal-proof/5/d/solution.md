<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The pivot columns in the [row echelon form](../../../../../row-echelon-form.md) are columns 1 and 2. Take the corresponding columns of the **original** [matrix](../../../../../matrix.md):

$$
\boxed{\operatorname{Col}(A)\text{ has basis }\left\{\begin{pmatrix}1\\2\\2\\0\end{pmatrix},\begin{pmatrix}1\\3\\0\\1\end{pmatrix}\right\}.}
$$

For a direct check, call these columns $c_1,c_2$. The other columns satisfy $c_3=c_1-c_2$ and $c_4=c_1+c_2$, so they are in the same [linear span](../../../../../linear-span.md). Also $c_1,c_2$ are [linearly independent](../../../../../linear-independence.md): their fourth entries force the coefficient of $c_2$ to vanish, then their first entries force the other coefficient to vanish. [Elementary row operations](../../../../../elementary-row-operation.md) preserve dependence relations among columns, but generally change the [column space](../../../../../column-space.md) itself, which is why the original columns must be used.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
