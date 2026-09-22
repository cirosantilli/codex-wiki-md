<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Gauss-Seidel method](../../../../../../gauss-seidel-method.md) solves each component using the already updated components from the same iteration. In the splitting $A=D-L-U$, those updated diagonal and lower-triangular terms stay on the left, while upper-triangular terms use the previous iterate. Thus

$$
\boxed{(D-L)x_n=Ux_{n-1}+b.}
$$

Here $D-L$ is lower triangular with nonzero diagonal, so each new iterate is obtained by [forward substitution](../../../../../../forward-substitution.md), starting from the specified zero vector.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
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
