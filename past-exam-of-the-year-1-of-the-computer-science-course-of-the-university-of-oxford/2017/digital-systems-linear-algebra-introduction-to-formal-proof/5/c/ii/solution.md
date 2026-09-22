<h1 id="5/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Introduce $z=Ux$. Solve $Lz=b$ by [forward substitution](../../../../../../forward-substitution.md) and then $Ux=z$ by [back substitution](../../../../../../back-substitution.md). For these factors, the recurrences are

$$
z_1=b_1,\quad z_2=b_2-z_1,\quad z_3=b_3-4z_2,
$$

followed by

$$
x_3=-z_3/4,\quad x_2=z_2-2x_3,\quad x_1=z_1-x_2-x_3.
$$

The nonzero diagonal entries make both triangular solves well-defined. No matrix inverse is calculated.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
