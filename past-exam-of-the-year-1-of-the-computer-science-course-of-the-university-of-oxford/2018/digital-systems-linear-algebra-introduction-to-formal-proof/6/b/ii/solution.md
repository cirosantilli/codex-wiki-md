<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The line passes through $p=(0,1)^T$ and has the same direction as in part (i). Translate by $-p$, reflect by $H$, then translate back. In [homogeneous coordinates](../../../../../../homogeneous-coordinate.md) the [affine reflection](../../../../../../reflection-in-an-affine-hyperplane.md) is

$$
\boxed{\begin{pmatrix}1&0&0\\0&1&1\\0&0&1\end{pmatrix}\begin{pmatrix}-7/25&24/25&0\\24/25&7/25&0\\0&0&1\end{pmatrix}\begin{pmatrix}1&0&0\\0&1&-1\\0&0&1\end{pmatrix}=\begin{pmatrix}-7/25&24/25&-24/25\\24/25&7/25&18/25\\0&0&1\end{pmatrix}.}
$$

Act on column $(x,y,1)^T$, reading the product from right to left. Every point with $y=4x/3+1$ is fixed. The translation column is $p-Hp$, as for any [reflection in an affine hyperplane](../../../../../../reflection-in-an-affine-hyperplane.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
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
