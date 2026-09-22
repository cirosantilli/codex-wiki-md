<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For eigenvalue zero take $s_1=(1,0)^T$. For eigenvalue $3/8$, the first row of $(B-3I/8)s_2=0$ gives $x=-2y$, so take $s_2=(-2,1)^T$. These are [linearly independent](../../../../../../linear-independence.md) [eigenvectors](../../../../../../eigenvector.md), giving

$$
\boxed{S=\begin{pmatrix}1&-2\\0&1\end{pmatrix},\quad
S^{-1}=\begin{pmatrix}1&2\\0&1\end{pmatrix},\quad
D=\begin{pmatrix}0&0\\0&3/8\end{pmatrix}.}
$$

The identities $Bs_i=\lambda_i s_i$ give $BS=SD$, hence the required [diagonalization](../../../../../../diagonalization-of-a-matrix.md) $S^{-1}BS=D$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
