# Lagrange leading-coefficient identity

↑ **Parent:** [Lagrange polynomial](lagrange-polynomial.md)

For $n+1$ distinct [interpolation nodes](interpolation-node.md) and an integer $0\leq k\leq n$,

$$
\sum_{i=0}^n\frac{x_i^k}{\prod_{j\ne i}(x_i-x_j)}
=\begin{cases}0,&k<n,\\1,&k=n.\end{cases}
$$

To prove this, the [Lagrange interpolation polynomial](lagrange-polynomial.md) for the data $x_i^k$ is exactly $x^k$, by uniqueness of [polynomial interpolation](polynomial-interpolation.md). The coefficient of $x^n$ in its $i$th [Lagrange cardinal polynomial](lagrange-cardinal-polynomial.md) is $1/\prod_{j\ne i}(x_i-x_j)$. Comparing the coefficients of $x^n$ gives the identity. At $k=0$, values of the constant [polynomial](polynomial-split.md) $1$ are intended even at a zero node. Negative exponents are outside the assertion.

## ↑ Ancestors (8)

1. [Lagrange polynomial](lagrange-polynomial.md)
2. [Polynomial interpolation](polynomial-interpolation.md)
3. [Interpolation](interpolation-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2023/2/b/solution.md)
