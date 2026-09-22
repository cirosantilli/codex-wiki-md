<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Rotate the specified line onto the horizontal axis, stretch horizontally by two while leaving the [orthogonal](../../../../../orthogonal-vectors.md) component unchanged, then rotate back. With $\theta=\pi/3$ and counterclockwise [rotation matrix](../../../../../rotation-matrix.md) $R(\theta)$, the requested product is

$$
\boxed{T=R(\theta)\begin{pmatrix}2&0\\0&1\end{pmatrix}R(-\theta)
=\begin{pmatrix}5/4&\sqrt3/4\\\sqrt3/4&7/4\end{pmatrix}.}
$$

The rightmost [rotation](../../../../../rotation-mathematics.md) acts first. In particular, $R(\theta)=\begin{pmatrix}1/2&-\sqrt3/2\\\sqrt3/2&1/2\end{pmatrix}$ and $R(-\theta)=R(\theta)^T$. For the unit direction $u=(1/2,\sqrt3/2)^T$, the same transformation is $T=I+uu^T$. It sends $u$ to $2u$ and fixes every [orthogonal](../../../../../orthogonal-vectors.md) [vector](../../../../../vector.md), verifying that the product is a [directional stretch](../../../../../directional-stretch.md) rather than a [shear mapping](../../../../../shear-mapping.md) or scaling in every direction. The constructed second panel in the geometric figure in Question 5 illustrates this separation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
