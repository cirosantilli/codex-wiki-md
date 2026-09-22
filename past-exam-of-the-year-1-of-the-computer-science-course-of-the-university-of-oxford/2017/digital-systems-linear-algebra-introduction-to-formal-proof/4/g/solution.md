<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Substitute the [QR decomposition](../../../../../qr-decomposition.md) into the [normal equations](../../../../../normal-equation.md):

$$
R^TRy=R^TQ^Tb.
$$

The diagonal of $R$ is nonzero, so $R^T$ is invertible. Cancel it algebraically to obtain

$$
\boxed{Ry=Q^Tb.}
$$

Compute the three [inner products](../../../../../inner-product-split.md) in $Q^Tb$, then use [back substitution](../../../../../back-substitution.md) in this [upper triangular matrix](../../../../../upper-triangular-matrix.md). There is no need to form an inverse or explicitly construct $A^TA$. The [orthogonal projection](../../../../../orthogonal-projection.md) of $b$ onto the column space is $QQ^Tb$; its orthogonal residual proves that this solution minimizes $\|Ay-b\|_2$.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
