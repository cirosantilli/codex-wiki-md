<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A generic lower triangular matrix has a dense first column. The first left [Householder transformation](../../../../householder-transformation.md) in its [QR decomposition](../../../../qr-decomposition.md) mixes those rows, usually creating entries throughout the rows to the right. Subsequent eliminations impose upper triangularity but no further systematic zeros; thus $R$ is generically a full upper triangular matrix.

For [Householder bidiagonalization](../../../../householder-bidiagonalization.md) use two-sided operations instead. At stage $j$, a right [Householder transformation](../../../../householder-transformation.md) acting on columns $j,\ldots,n$ clears the current row $j$ beyond its diagonal. Then a left [Householder transformation](../../../../householder-transformation.md) acting on rows $j+1,\ldots,n$ clears column $j$ below its first subdiagonal. The left operation leaves row $j$ unchanged; both operations preserve the already completed lower-bidiagonal rows and columns. Continue for $j=1,\ldots,n-1$, omitting a final unnecessary left operation. The result is

$$
\boxed{B=PAQ,\qquad P,Q\text{ orthogonal},\quad B\text{ lower bidiagonal}.}
$$

It follows that $B^TB=Q^TA^TAQ$. Hence the two symmetric matrices are [orthogonally similar](../../../../orthogonal-similarity.md) and have the same [eigenvalues](../../../../eigenvalue.md). By part (c), compute the [eigenvalues](../../../../eigenvalue.md) of the symmetric [tridiagonal matrix](../../../../tridiagonal-matrix.md) $B^TB$ and take their nonnegative square roots to obtain all [singular values](../../../../singular-value.md) of $A$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
