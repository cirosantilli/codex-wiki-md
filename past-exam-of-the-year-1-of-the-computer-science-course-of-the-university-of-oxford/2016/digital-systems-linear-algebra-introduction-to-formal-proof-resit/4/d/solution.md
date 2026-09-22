<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The first two columns are already orthogonal and have norms 15 and 5. Their normalized versions are $q_1=(3,4,0,0)^T/5$ and $q_2=(0,0,4,-3)^T/5$. Their [inner products](../../../../../inner-product-split.md) with the third column are 10 and 5. Subtracting these projections leaves $(20,-15,0,0)^T$, whose norm is 25. Thus an economy-size [QR factorization](../../../../../qr-decomposition.md) is

$$
\boxed{Q=\frac15\begin{pmatrix}3&0&4\\4&0&-3\\0&4&0\\0&-3&0\end{pmatrix},\qquad R=\begin{pmatrix}15&0&10\\0&5&5\\0&0&25\end{pmatrix}.}
$$

Direct multiplication gives $Q^TQ=I_3$ and $QR=A$. If a full square $Q$ is required, append $q_4=(0,0,3,4)^T/5$ and append a zero fourth row to $R$; the product is unchanged and the completed $Q$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
