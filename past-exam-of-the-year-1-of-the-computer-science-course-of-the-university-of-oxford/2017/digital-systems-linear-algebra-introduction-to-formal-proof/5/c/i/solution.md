<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First subtract row one from row two, using $E_1$; then subtract four times the updated row two from row three, using $E_2$:

$$
E_1=\begin{pmatrix}1&0&0\\-1&1&0\\0&0&1\end{pmatrix},\qquad
E_2=\begin{pmatrix}1&0&0\\0&1&0\\0&-4&1\end{pmatrix}.
$$

The updated second row is $(0,1,2)$ and the final third row is $(0,0,-4)$. Hence $E_2E_1A=U$ and $L=E_1^{-1}E_2^{-1}$. The resulting [LU decomposition](../../../../../../lu-decomposition.md) is

$$
\boxed{L=\begin{pmatrix}1&0&0\\1&1&0\\0&4&1\end{pmatrix},\qquad
U=\begin{pmatrix}1&1&1\\0&1&2\\0&0&-4\end{pmatrix},\qquad A=LU.}
$$

Reversing the order when undoing the elementary operations is essential.

## ↑ Ancestors (13)

1. [I](../i.md)
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
