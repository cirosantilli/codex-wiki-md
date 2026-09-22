<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For independent columns $a_1,\ldots,a_k$ in a real [inner product space](../../../../../../inner-product-space.md), the [Gram-Schmidt process](../../../../../../gram-schmidt-process.md) recursively forms

$$
u_j=a_j-\sum_{i<j}\langle q_i,a_j\rangle q_i,\qquad q_j=\frac{u_j}{\|u_j\|}.
$$

Each $u_j$ subtracts the [orthogonal projections](../../../../../../orthogonal-projection.md) onto earlier normalized vectors. Their independence ensures $u_j\ne0$. The resulting $q_i$ are [orthonormal](../../../../../../orthonormal-set.md) and preserve the span of every initial column set. Putting $Q=(q_1\ \cdots\ q_k)$ and $r_{ij}=\langle q_i,a_j\rangle$ for $i\leq j$, with zeros below the diagonal, gives a [QR decomposition](../../../../../../qr-decomposition.md) $A=QR$ with $Q^TQ=I$. Dependent input columns require omitting a zero residual or treating rank deficiency separately.

## ↑ Ancestors (13)

1. [I](../i.md)
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
