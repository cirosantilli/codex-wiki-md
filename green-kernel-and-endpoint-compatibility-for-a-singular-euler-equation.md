# Green kernel and endpoint compatibility for a singular Euler equation

↑ **Parent:** [Green's function](green-s-function-split.md)

For $0<x<1$, the homogeneous [Cauchy-Euler equation](cauchy-euler-equation.md) has solutions $x,x^{-1}$. The left-vanishing solution $x$ and right-vanishing solution $x-x^{-1}$ give the unweighted [Green function](green-s-function-split.md) $G(x,s)=x(1-s^{-2})/2$ for $x\leq s$ and $(x-x^{-1})/2$ for $x\geq s$. It is continuous at $x=s$ and its first derivative has jump $1/s^2$, so $L_xG=\delta(x-s)$.

For continuous forcing $f$ on $[0,1]$, its integral is

$$
u(x)=\frac{x-x^{-1}}2\int_0^xf(s)ds+\frac x2\int_x^1(1-s^{-2})f(s)ds.
$$

This is bounded at zero and vanishes at one, but $u(0^+)=-f(0)$. The first singular term uses the average $x^{-1}\int_0^xf\to f(0)$. In the other, the substitution $t=x/s$ gives $x\int_x^1f(s)s^{-2}ds=\int_x^1f(x/t)dt\to f(0)$ by [dominated convergence](dominated-convergence-theorem.md). Thus the two zero endpoint values require $f(0)=0$. When compatible, the solution is unique among bounded solutions because no nonzero combination of $x,x^{-1}$ meets both homogeneous endpoint conditions. This example shows why pointwise endpoint behavior of a [Green function](green-s-function-split.md) does not itself justify passing a limit through its integral.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1/3/solution.md)
