<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $A$, the [triangular matrix](../../../../../triangular-matrix.md) formula gives the [characteristic polynomial](../../../../../characteristic-polynomial.md)

$$
\det(tI-A)=(t-1)(t-3)(t-2).
$$

The three [eigenvalues](../../../../../eigenvalue.md) are distinct, so part (d) already proves the existence of an [eigenvector](../../../../../eigenvector.md) [basis](../../../../../basis.md). Explicit choices, ordered by [eigenvalues](../../../../../eigenvalue.md) $1,3,2$, are

$$
\boxed{(1,0,0)^T,\quad(1,1,0)^T,\quad(2,-1,1)^T.}
$$

Their column [matrix](../../../../../matrix.md) has [determinant](../../../../../determinant.md) one, and direct multiplication gives respectively one, three and two times the indicated [vector](../../../../../vector.md).

For $B$, expansion along the last row gives

$$
\det(tI-B)=(t-3)((t-3)^2-1)=(t-3)(t-4)(t-2).
$$

Again the three [eigenvalues](../../../../../eigenvalue.md) are distinct. An explicit [eigenvector](../../../../../eigenvector.md) [basis](../../../../../basis.md), ordered by [eigenvalues](../../../../../eigenvalue.md) $4,2,3$, is

$$
\boxed{(1,1,0)^T,\quad(1,-1,0)^T,\quad(0,-1,1)^T.}
$$

Its column [matrix](../../../../../matrix.md) has [determinant](../../../../../determinant.md) $-2\ne0$. In particular, $B$'s diagonal entries are not its [eigenvalues](../../../../../eigenvalue.md): it is not a [triangular matrix](../../../../../triangular-matrix.md).

Finally $C=I_3$, so every nonzero [vector](../../../../../vector.md) is an [eigenvector](../../../../../eigenvector.md) with [eigenvalue](../../../../../eigenvalue.md) one. Choose **the [standard basis](../../../../../standard-basis.md) $e_1,e_2,e_3$**. These are [linearly independent](../../../../../linear-independence.md) even though their [eigenvalues](../../../../../eigenvalue.md) coincide. Distinct [eigenvalues](../../../../../eigenvalue.md) are sufficient for an [eigenvector](../../../../../eigenvector.md) [basis](../../../../../basis.md), and are not necessary.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
