<h1 id="5/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $f_j$ be the [determinant](../../../../../../determinant.md) of the leading $j\times j$ [principal submatrix](../../../../../../principal-submatrix.md). Expansion along the last row gives an $a_jf_{j-1}$ term and a $c_{j-1}$ term with negative [cofactor](../../../../../../cofactor.md) sign. In the latter minor, the final column has only $b_{j-1}$ nonzero, and deleting that row and column leaves the leading $(j-2)\times(j-2)$ [principal submatrix](../../../../../../principal-submatrix.md). Thus the [tridiagonal determinant recurrence](../../../../../../tridiagonal-determinant-recurrence.md) is

$$
\boxed{f_0=1,\qquad f_1=a_1,\qquad f_j=a_jf_{j-1}-c_{j-1}b_{j-1}f_{j-2}\quad(j\ge2).}
$$

Here $f_0=1$ is the empty [determinant](../../../../../../determinant.md) convention, needed to include $f_2=a_1a_2-b_1c_1$. The derivation uses [cofactor expansion](../../../../../../laplace-expansion.md), so the [recurrence relation](../../../../../../recurrence-relation.md) remains valid when coefficients or intermediate [determinants](../../../../../../determinant.md) vanish; it never divides by a [pivot element](../../../../../../pivot-element.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
