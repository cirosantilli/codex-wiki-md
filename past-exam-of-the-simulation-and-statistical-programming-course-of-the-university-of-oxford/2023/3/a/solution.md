<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The following [R](../../../../r-programming-language.md) code implements the given [recursion](../../../../recursion-computer-science.md) for the [Cholesky decomposition](../../../../cholesky-decomposition.md). The input is assumed to be a real [symmetric matrix](../../../../symmetric-matrix.md) that is a [positive-definite matrix](../../../../positive-definite-matrix.md).

```
mychol <- function(A) {
  n <- nrow(A)
  if (n == 1L) return(matrix(sqrt(A[1L, 1L]), 1L, 1L))
  j <- 2L:n
  L <- matrix(0, n, n)
  L[1L, 1L] <- sqrt(A[1L, 1L])
  b <- A[j, 1L, drop = FALSE] / L[1L, 1L]
  L[j, 1L] <- b
  S <- A[j, j, drop = FALSE] - tcrossprod(b)
  L[j, j] <- mychol(S)
  L
}
```

Here `tcrossprod(b)` is the [outer product](../../../../outer-product.md) $bb^T$. The `drop = FALSE` arguments preserve [matrix](../../../../matrix.md) dimensions, including the final one-by-one subproblem, and the [base case](../../../../base-case.md) also returns a [matrix](../../../../matrix.md).

To verify correctness, partition $A=\begin{pmatrix}a&r^T\\r&B\end{pmatrix}$. The code sets $\ell=\sqrt a$, $b=r/\ell$ and recursively factors $S=B-bb^T$. This [Schur complement](../../../../schur-complement.md) is a [positive-definite matrix](../../../../positive-definite-matrix.md): for $z\ne0$,

$$
z^TSz=
\begin{pmatrix}-r^Tz/a\\z\end{pmatrix}^{\!T}
A
\begin{pmatrix}-r^Tz/a\\z\end{pmatrix}>0.
$$

If $CC^T=S$ is the recursive answer, then the returned [lower triangular matrix](../../../../lower-triangular-matrix.md) satisfies

$$
L=\begin{pmatrix}\ell&0\\b&C\end{pmatrix},
\qquad
LL^T=\begin{pmatrix}a&\ell b^T\\\ell b&bb^T+CC^T\end{pmatrix}
=\begin{pmatrix}a&r^T\\r&B\end{pmatrix}=A.
$$

The one-dimensional identity starts this [mathematical induction](../../../../mathematical-induction.md) proof. Each recursive call reduces the [matrix](../../../../matrix.md) size by one and therefore terminates.

## ↑ Ancestors (12)

1. [A](../a.md)
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
