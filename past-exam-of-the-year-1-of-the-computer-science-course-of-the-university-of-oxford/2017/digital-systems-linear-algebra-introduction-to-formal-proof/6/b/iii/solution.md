<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The exact solution obeys $(D-L)x=Ux+b$. Subtract this from the iteration to get $(D-L)e_n=Ue_{n-1}$. Hence the [stationary iteration matrix](../../../../../../iteration-matrix.md) is

$$
\boxed{G=(D-L)^{-1}U
=\begin{pmatrix}1/4&0\\-1/8&1/2\end{pmatrix}
\begin{pmatrix}0&-3\\0&0\end{pmatrix}
=\begin{pmatrix}0&-3/4\\0&3/8\end{pmatrix},\qquad e_n=Ge_{n-1}.}
$$

This is exactly the matrix $B$ from part (a); the sign follows the given $A=D-L-U$ convention.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
