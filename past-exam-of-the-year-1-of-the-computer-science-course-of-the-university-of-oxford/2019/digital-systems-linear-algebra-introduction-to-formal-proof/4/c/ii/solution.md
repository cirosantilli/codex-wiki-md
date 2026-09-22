<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the same permutation to the right-hand side and solve two [triangular systems](../../../../../../triangular-system.md). [Forward substitution](../../../../../../forward-substitution.md) in $Ly=Pb$ gives

$$
y_1=3,\qquad 2y_1+y_2=0,\qquad3y_1+y_3=-2,
$$

so $y=(3,-6,-11)^T$. [Back substitution](../../../../../../back-substitution.md) in $Ux=y$ gives $-11x_3=-11$, $4x_2-2x_3=-6$, and $3x_1+x_2+4x_3=3$. Therefore **$x=(0,-1,1)^T$**. Substitution in the original system returns $(3,-2,0)^T$, as required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
