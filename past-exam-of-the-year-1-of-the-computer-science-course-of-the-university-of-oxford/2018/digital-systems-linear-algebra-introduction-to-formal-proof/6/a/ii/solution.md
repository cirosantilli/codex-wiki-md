<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The first column has norm two, giving $q_1=(1,-1,1,-1)^T/2$. Its inner products with the second and third columns are both one. Subtracting $q_1$ from the second column leaves $(3,3,3,3)^T/2$, of norm three, so $q_2=(1,1,1,1)^T/2$. The inner product of $q_2$ with the third column is one. Subtracting $q_1+q_2$ from that column leaves $(1,1,-1,-1)^T$, of norm two. Thus the [Gram-Schmidt process](../../../../../../gram-schmidt-process.md) gives

$$
\boxed{Q=\frac12\begin{pmatrix}1&1&1\\-1&1&1\\1&1&-1\\-1&1&-1\end{pmatrix},\qquad R=\begin{pmatrix}2&1&1\\0&3&1\\0&0&2\end{pmatrix}.}
$$

The columns of $Q$ have unit norm and pairwise zero [inner products](../../../../../../inner-product-split.md), so $Q^TQ=I_3$. Direct multiplication verifies $QR=A$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
