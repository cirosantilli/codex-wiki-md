# Thin QR factorization from Cholesky decomposition

↑ **Parent:** [QR decomposition](qr-decomposition.md)

If a real $m$-by-$n$ matrix $A$ has full column rank, with $m\ge n$, then $A^TA$ is [positive-definite](positive-definite-bilinear-form.md). Its upper-triangular [Cholesky decomposition](cholesky-decomposition.md) $A^TA=R^TR$, with positive diagonal, is unique. Defining $Q=AR^{-1}$ gives $Q^TQ=I$ and $A=QR$. Any other such factorization yields another Cholesky factor of $A^TA$, so its $R$ and then its $Q$ must agree. This proves existence and uniqueness; it does not assert that forming $A^TA$ is the most numerically stable algorithm.

## ↑ Ancestors (8)

1. [QR decomposition](qr-decomposition.md)
2. [Gram-Schmidt process](gram-schmidt-process.md)
3. [Inner product](inner-product.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/14e/b/solution.md)
