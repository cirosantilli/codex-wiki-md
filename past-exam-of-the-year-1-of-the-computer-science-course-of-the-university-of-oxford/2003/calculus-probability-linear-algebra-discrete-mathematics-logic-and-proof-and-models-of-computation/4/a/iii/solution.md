<h1 id="4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If a square [matrix](../../../../../../matrix.md) $A$ is an [invertible matrix](../../../../../../invertible-matrix.md), [multiplicativity of the determinant](../../../../../../multiplicativity-of-the-determinant.md) gives

$$
1=\det I=\det(AA^{-1})=(\det A)(\det A^{-1}),
$$

so $\det A\ne0$.

Conversely, suppose $\det A\ne0$. Use [Gaussian elimination](../../../../../../gaussian-elimination.md) to reduce $A$ to [row echelon form](../../../../../../row-echelon-form.md) $U$. Each [elementary row operation](../../../../../../elementary-row-operation.md) multiplies the [determinant](../../../../../../determinant.md) by a nonzero factor, so $\det U\ne0$. If this square [matrix](../../../../../../matrix.md) had fewer than $n$ [pivots](../../../../../../pivotal-quantity.md), its [row echelon form](../../../../../../row-echelon-form.md) would have a zero row and hence zero [determinant](../../../../../../determinant.md), a contradiction. Therefore it has a [pivot](../../../../../../pivotal-quantity.md) in every row and column, and further [elementary row operations](../../../../../../elementary-row-operation.md) reduce it to $I$.

Each [elementary row operation](../../../../../../elementary-row-operation.md) is multiplication on the left by an [invertible matrix](../../../../../../invertible-matrix.md), its inverse being the reverse operation. Thus $E_k\cdots E_1A=I$ implies $A=E_1^{-1}\cdots E_k^{-1}$, a product of [invertible matrices](../../../../../../invertible-matrix.md). Hence

$$
\boxed{A\text{ is invertible}\iff\det A\ne0.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
