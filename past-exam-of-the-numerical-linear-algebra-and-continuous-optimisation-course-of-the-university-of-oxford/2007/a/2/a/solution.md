<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Direct solution usually uses a pivoted [LU decomposition](../../../../../lu-decomposition.md) $PA=LU$: solve $Lz=Pb$ by [forward substitution](../../../../../forward-substitution.md), then $Ux=z$ by [back substitution](../../../../../back-substitution.md). For a [symmetric positive-definite matrix](../../../../../symmetric-positive-definite-matrix.md), the [Cholesky decomposition](../../../../../cholesky-decomposition.md) is

$$
\boxed{A=CC^T,}
$$

with $C$ lower triangular and positive diagonal. It exploits symmetry, requiring about $n^3/3$ arithmetic operations rather than the leading $2n^3/3$ for general elimination.

If $A$ has full column rank and its reduced [QR decomposition](../../../../../qr-decomposition.md) is $A=QR$, $Q^TQ=I$, then

$$
\boxed{A^TA=R^TR.}
$$

Choose the signs of $Q,R$ so that $R$ has positive diagonal. Then $R$ is precisely the upper [Cholesky factor](../../../../../cholesky-factor.md) of the normal-equation matrix $A^TA$, or $R^T$ is its lower factor. This identifies the factors; in computation, obtaining $R$ directly by [QR decomposition](../../../../../qr-decomposition.md) avoids explicitly forming the [normal equations](../../../../../normal-equation.md), which square the condition number.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
