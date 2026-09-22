# Chebyshev-Lobatto node

↑ **Parent:** [Interpolation node](interpolation-node.md)

For $n\geq1$, the $n+1$ [Chebyshev-Lobatto nodes](chebyshev-lobatto-node.md) are the [extrema](maximum-and-minimum.md) of the [Chebyshev polynomial](chebyshev-polynomial.md) $T_n$ on $[-1,1]$, including both endpoints: $T_n(x_k)=(-1)^k$. Imagine $n+1$ equally spaced angles on a [semicircle](semicircle.md) and project their points onto the horizontal axis. The [interpolation nodes](interpolation-node.md) crowd near $-1$ and $1$ because equal angular steps have smaller horizontal projections there. Reversing the order gives the same set. These are distinct from the [roots of a polynomial](root-of-a-polynomial.md) $\cos((2k+1)\pi/(2n+2))$ of $T_{n+1}$, which omit the endpoints. Driscoll and Braun call this endpoint-including family Chebyshev points of the second kind or Chebyshev extreme points.[Driscoll and Braun, Fundamentals of Numerical Computation, §9.3.2, equation 9.3.2](https://fncbook.com/python/stability-1/)

On an interval $[a,b]$, use $x_k=(a+b)/2+(b-a)\cos(k\pi/n)/2$. The [Runge phenomenon](runge-s-phenomenon.md) example compares [polynomial interpolation](polynomial-interpolation.md) at eleven [Chebyshev-Lobatto nodes](chebyshev-lobatto-node.md) with eleven equally spaced [interpolation nodes](interpolation-node.md). The distinction matters whenever sampling locations are a choice rather than fixed observations.

## ↑ Ancestors (8)

1. [Interpolation node](interpolation-node.md)
2. [Polynomial interpolation](polynomial-interpolation.md)
3. [Interpolation](interpolation.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Chebyshev-Lobatto node](chebyshev-lobatto-node.md)
- [Chebyshev polynomial](chebyshev-polynomial.md)
- [Runge's phenomenon](runge-s-phenomenon.md)
