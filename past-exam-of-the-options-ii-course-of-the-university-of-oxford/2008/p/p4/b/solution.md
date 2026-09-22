<h1 id="p/p4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Only the first and third coordinates occur in the first two columns. Normalize the first column to get $q_1=(4,0,3,0)^T/5$. Removing its component from the second column leaves $(21,0,-28,0)^T/5$, of length seven, so $q_2=(3,0,-4,0)^T/5$. The remaining orthonormal columns can be $q_3=e_2$ and $q_4=e_4$. Taking their dot products with the columns of $A$ gives

$$
\boxed{Q=\begin{pmatrix}4/5&3/5&0&0\\0&0&1&0\\3/5&-4/5&0&0\\0&0&0&1\end{pmatrix},\qquad
R=\begin{pmatrix}5&1&5&2\\0&7&10&-11\\0&0&9&6\\0&0&0&1\end{pmatrix}}.
$$

The columns of $Q$ are orthonormal, and direct multiplication gives the source matrix. Exploiting its two-coordinate first block avoids unnecessary four-dimensional elimination.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
