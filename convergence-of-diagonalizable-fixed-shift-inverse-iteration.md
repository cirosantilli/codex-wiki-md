# Convergence of diagonalizable fixed-shift inverse iteration

↑ **Parent:** [Inverse iteration](inverse-iteration.md)

Suppose a [diagonalizable matrix](diagonalizable-matrix.md) has a simple [eigenvalue](eigenvalue.md) $\lambda_*$ uniquely closest to a shift $\mu\notin\operatorname{spec}(A)$. If the starting [vector](vector.md) has a nonzero coefficient $c_*$ in the target [eigenbasis](eigenbasis.md) direction, fixed-shift [inverse iteration](inverse-iteration.md) converges to that [eigenvector](eigenvector.md) line. In fact, the [eigenvalues](eigenvalue.md) of $(A-\mu I)^{-1}$ are $(\lambda_j-\mu)^{-1}$, so after $k$ inverse applications, division by $c_*(\lambda_*-\mu)^{-k}$ leaves the target [eigenvector](eigenvector.md) plus

$$
\sum_{j\ne *}\frac{c_j}{c_*}
\left(\frac{\lambda_*-\mu}{\lambda_j-\mu}\right)^ku_j.
$$

This proves direction error $O(q_\mu^k)$ in [Big O notation](big-o-notation.md). The multiplicative constant depends on the [eigenbasis](eigenbasis.md) and starting coefficients, and no uniform reduction at the first step follows for a [nonsymmetric matrix](nonsymmetric-matrix.md). Over the real numbers, $\lambda_*<\mu$ produces alternating signs. A nonzero ordinary [inner product](inner-product-split.md) with a right [eigenvector](eigenvector.md) is not generally the same as a nonzero coefficient in the [eigenbasis](eigenbasis.md); the latter is the required condition.

## ↑ Ancestors (8)

1. [Inverse iteration](inverse-iteration.md)
2. [Power method](power-method.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2023/1/c/solution.md)
