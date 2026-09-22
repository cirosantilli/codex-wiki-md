# Euler proof that the sum of reciprocals of primes diverges

↑ **Parent:** [Euler product](euler-product.md)

For a finite set of primes,

$$
\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
$$

expands as the sum of $1/n$ over positive integers whose prime factors are at most $x$. It contains every term with $n\leq x$, so these partial products dominate the [harmonic series](harmonic-series.md) and diverge. Since

$$
-\log(1-t)=t+O(t^2)
$$

uniformly for $0\leq t\leq1/2$, convergence of $\sum_p1/p$ would force convergence of the logarithms of these products, a contradiction.

**Table of contents**

- [Prime reciprocal lower bound](prime-reciprocal-lower-bound.md)

## ↑ Ancestors (7)

1. [Euler product](euler-product.md)
2. [Dirichlet series](dirichlet-series.md)
3. [Analytic number theory](analytic-number-theory-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Brun's theorem](brun-s-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/1i/solution.md)
