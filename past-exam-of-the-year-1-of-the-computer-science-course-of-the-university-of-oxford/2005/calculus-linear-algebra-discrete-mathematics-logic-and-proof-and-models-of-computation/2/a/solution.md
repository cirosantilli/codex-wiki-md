<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The printed word “eigenvalues” must read “eigenvectors”: [eigenvalues](../../../../../eigenvalue.md) are real numbers, whereas a [basis](../../../../../basis.md) of $\mathbb R^n$ consists of [vectors](../../../../../vector.md). The intended assertion is

$$
\boxed{A\text{ is diagonalizable over }\mathbb R\iff\mathbb R^n\text{ has a basis of eigenvectors of }A.}
$$

This wording error is present in the original scan.[Printed p. 2, Q2(a), “basis consisting of eigenvalues”](../../../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-examination-paper-by-the-university-of-oxford-2005.md)

If $X^{-1}AX=D=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)$ for an [invertible matrix](../../../../../invertible-matrix.md) $X$, write $x_i$ for its columns. The [matrix](../../../../../matrix.md) identity $AX=XD$ says $Ax_i=\lambda_ix_i$. The columns of an [invertible matrix](../../../../../invertible-matrix.md) are a [basis](../../../../../basis.md), hence they give the required [basis](../../../../../basis.md) of [eigenvectors](../../../../../eigenvector.md).

Conversely, put a [basis](../../../../../basis.md) of real [eigenvectors](../../../../../eigenvector.md) $x_1,\ldots,x_n$ into the columns of $X$, with corresponding [eigenvalues](../../../../../eigenvalue.md) $\lambda_i$. The [basis](../../../../../basis.md) property makes $X$ an [invertible matrix](../../../../../invertible-matrix.md). The equations $Ax_i=\lambda_ix_i$ give $AX=XD$, so $X^{-1}AX=D$. This is precisely [diagonalizability](../../../../../diagonalizable-matrix.md) over the real numbers.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
