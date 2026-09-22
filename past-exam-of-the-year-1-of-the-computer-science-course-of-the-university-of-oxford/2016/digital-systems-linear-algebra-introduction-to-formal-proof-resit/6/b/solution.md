<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the original rows be $r_1,\ldots,r_5$. Begin with rows $r_2$, $r_3-r_2$ and $r_4$:

$$
(1,1,0,0),\qquad(0,1,1,0),\qquad(0,0,1,1).
$$

Subtract the third from the second, then subtract that new second row from the first. The resulting rows are

$$
\boxed{(1,0,0,1),\quad(0,1,0,-1),\quad(0,0,1,1).}
$$

They are linearly independent because their first three coordinates form the [identity matrix](../../../../../identity-matrix.md). All original rows lie in their span: $r_1=2r_2+r_4$ and $r_5=r_2-(r_3-r_2)+r_4$. Thus they form a [basis](../../../../../basis.md) of the [row space](../../../../../row-space.md), and **$\operatorname{rank}A=3$**. Equivalently, these are the nonzero rows of the reduced row echelon form, with two further zero rows.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
