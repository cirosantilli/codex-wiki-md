<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Cholesky decomposition](../../../../../cholesky-decomposition.md) gives $\Sigma=LL^T$. If $B=L^{-1}$, reversal of factors in a [matrix inverse](../../../../../matrix-inverse-split.md) gives

$$
\boxed{\Sigma^{-1}=(L^T)^{-1}L^{-1}=B^TB.}
$$

Hence the required [R](../../../../../r-programming-language.md) implementation is

```
invsigma <- function(sigma) {
  L <- mychol(sigma)
  B <- ltinv(L)
  crossprod(B)
}
```

Here `crossprod(B)` computes $B^TB$. Using `tcrossprod(B)` would compute $BB^T$, which generally differs from $\Sigma^{-1}$. Both helper functions preserve the one-by-one [matrix](../../../../../matrix.md) case.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
