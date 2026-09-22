<h1 id="chebyshev-gauss-quadrature">Chebyshev–Gauss quadrature</h1>

↑ **Parent:** [Gaussian quadrature](gaussian-quadrature.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev–Gauss_quadrature)

The first-kind rule approximates $\int_{-1}^1 f(x)(1-x^2)^{-1/2}\,dx$ at the zeros of the [Chebyshev polynomial](chebyshev-polynomial.md) $T_n$. It integrates all [polynomials](polynomial-split.md) of degree at most $2n-1$ exactly. The weights follow by integrating the [Lagrange interpolation polynomial](lagrange-polynomial.md) at those nodes. Orthogonality kills the quotient when a degree-$2n-1$ polynomial is divided by $T_n$; its remainder is recovered by interpolation. No $n$-node rule can integrate every degree-$2n$ polynomial, since the squared nodal polynomial has zero quadrature sum and strictly positive weighted integral.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (6)

1. [Gaussian quadrature](gaussian-quadrature.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/8d/solution.md)
