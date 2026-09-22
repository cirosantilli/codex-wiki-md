<h1 id="t/1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The entries in the two slack columns give the inverse basis [matrix](../../../../../../matrix.md)

$$
B^{-1}=\begin{pmatrix}1/3&-1/3\\1/3&2/3\end{pmatrix},\qquad
B=\begin{pmatrix}2&1\\-1&1\end{pmatrix}.
$$

Thus the ordered basic variables are $x_3,x_1$. Multiplying the original coefficient [matrix](../../../../../../matrix.md) and right-hand side by $B^{-1}$ gives the completed constraint rows. With the bottom row defined as reduced costs $c^T-c_B^TB^{-1}A$ and right-hand entry $-c_B^TB^{-1}b$, the complete tableau is

$$
\boxed{\begin{array}{rrrrr|r}
0&-1&1&1/3&-1/3&2/3\\
1&3&0&1/3&2/3&14/3\\\hline
0&-6&0&-1/3&-5/3&-26/3
\end{array}.}
$$

This bottom-right entry is the negative of the optimal objective under this row-operation convention. If a tableau records the positive objective value separately in that position, it is $26/3$; the completed constraint rows and reduced costs are the same.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [T](../../../../t.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options I course of the University of Oxford](../../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
