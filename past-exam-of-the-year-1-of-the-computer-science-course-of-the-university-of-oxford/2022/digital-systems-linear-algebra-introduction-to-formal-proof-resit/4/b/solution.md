<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [mathematical induction](../../../../../mathematical-induction.md) on $n$. For $n=0$, the identity [matrix](../../../../../matrix.md) gives $(1,2)^T=(L_1,L_0)^T$. If $A^n(1,2)^T=(L_{n+1},L_n)^T$, applying $A$ and using part (a) gives $A^{n+1}(1,2)^T=(L_{n+2},L_{n+1})^T$. Therefore

$$
\boxed{A^n\begin{pmatrix}1\\2\end{pmatrix}=\begin{pmatrix}L_{n+1}\\L_n\end{pmatrix}\quad(n\geq0).}
$$

The base case is essential: the starting vector represents consecutive [Lucas numbers](../../../../../lucas-number.md), not two arbitrary initial values.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
