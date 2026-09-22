<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [inverse matrix](../../../../matrix-inverse-split.md) exists only if the [lower triangular matrix](../../../../lower-triangular-matrix.md) has no zero [diagonal entries](../../../../diagonal-matrix-entry.md); this necessary assumption is implicit in the request for $L^{-1}$. Partition

$$
L=\begin{pmatrix}a&0\\b&C\end{pmatrix}.
$$

Writing its inverse in the same block form and multiplying gives the [recursive inverse of a lower triangular matrix](../../../../recursive-inverse-of-a-lower-triangular-matrix.md):

$$
\boxed{L^{-1}=\begin{pmatrix}a^{-1}&0\\-C^{-1}b/a&C^{-1}\end{pmatrix}.}
$$

Indeed the lower-left block of the product is $b/a-C(C^{-1}b/a)=0$, and the diagonal blocks are identities. This gives an implementation with no call to `solve`:

```
ltinv <- function(L) {
  n <- nrow(L)
  if (n == 1L) return(matrix(1 / L[1L, 1L], 1L, 1L))
  j <- 2L:n
  Cinv <- ltinv(L[j, j, drop = FALSE])
  B <- matrix(0, n, n)
  B[1L, 1L] <- 1 / L[1L, 1L]
  B[j, j] <- Cinv
  B[j, 1L] <- -as.vector(Cinv %*% L[j, 1L, drop = FALSE]) / L[1L, 1L]
  B
}
```

The preserved [matrix](../../../../matrix.md) dimensions also handle $n=2$. A [mathematical induction](../../../../mathematical-induction.md) using the block identity proves that every returned [matrix](../../../../matrix.md) is the desired inverse. Applied to the [Cholesky decomposition](../../../../cholesky-decomposition.md) from (a), all [diagonal entries](../../../../diagonal-matrix-entry.md) are positive, so all divisions are valid.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../split.md)
5. [Simulation and statistical programming course of the University of Oxford](../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
