# Hermite interpolation error formula

↑ **Parent:** [Hermite interpolation](hermite-interpolation.md)

Let $x_0<\cdots<x_n$ be distinct [interpolation nodes](interpolation-node.md), let $f\in C^{2n+2}[x_0,x_n]$, and let $H$ be the [Hermite interpolating polynomial](hermite-interpolating-polynomial.md) matching the values and first [derivatives](derivative.md) of $f$ at all nodes. For each $x$ in the interval there is an interior point $\xi$ for which the displayed formula holds. At a node the formula is immediate. Otherwise put $e=f-H$, $\pi(t)=\prod_i(t-x_i)$ and $\varphi(t)=e(t)-e(x)\pi(t)^2/\pi(x)^2$. This function vanishes at the $n+1$ nodes and at $x$, while its [derivative](derivative.md) vanishes at every node. [Rolle's theorem](rolle-theorem.md) gives $n+1$ additional zeros of its [derivative](derivative.md) between successive zeros of $\varphi$. Repeating the theorem therefore gives $\varphi^{(2n+2)}(\xi)=0$. Since $H^{(2n+2)}=0$ and $(\pi^2)^{(2n+2)}=(2n+2)!$, rearrangement yields the formula. The extra point $x$ is a zero of $\varphi$, not necessarily of its [derivative](derivative.md).

For two nodes $a,b$, this gives the uniform bound $\|f-H\|_\infty\le\|f^{(4)}\|_\infty(b-a)^4/384$, since $(x-a)^2(b-x)^2\le(b-a)^4/16$. The squared nodal factors encode simultaneous matching of values and [derivatives](derivative.md).

## ↑ Ancestors (6)

1. [Hermite interpolation](hermite-interpolation.md)
2. [Polynomial interpolation error](polynomial-interpolation-error.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2007/p/3/d/solution.md)
