<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $Q^{-1}=Q^T$, the [QR factorization](../../../../qr-decomposition.md) gives

$$
Ax=b\quad\Longleftrightarrow\quad Rx=Q^Tb.
$$

First compute $y=Q^Tb$ by a [matrix-vector product](../../../../matrix-vector-product.md), costing $n^2$ scalar multiplications and $n(n-1)$ additions for dense $Q$. Then solve the [upper triangular matrix](../../../../upper-triangular-matrix.md) system $Rx=y$ by [back substitution](../../../../back-substitution.md):

$$
\boxed{x_i=\frac{y_i-\sum_{j=i+1}^nr_{ij}x_j}{r_{ii}},\qquad i=n,n-1,\ldots,1.}
$$

Every denominator is nonzero because $R=Q^TA$ is invertible. The [back substitution](../../../../back-substitution.md) costs $n(n-1)$ multiplications and subtractions together, plus $n$ divisions, for $n^2$ [arithmetic operations](../../../../arithmetic-operation.md). Including $Q^Tb$, the total is $3n^2-n$ [arithmetic operations](../../../../arithmetic-operation.md) under this scalar counting convention, hence **$O(n^2)$**, with $O$ denoting [Big O notation](../../../../big-o-notation.md). The already supplied [QR factorization](../../../../qr-decomposition.md) is reused; no [matrix inverse](../../../../matrix-inverse-split.md) needs to be computed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
