# Sharp Peano-kernel constant for the three-point endpoint first derivative

↑ **Parent:** [Sharp error constants for a Peano kernel](sharp-error-constants-for-a-peano-kernel.md)

For $L(f)=f'(0)+\frac32f(0)-2f(1)+\frac12f(2)$ on $C^3[0,2]$, the [Peano kernel](peano-kernel.md) is

$$
K(t)=\begin{cases}t-\frac34t^2,&0\le t\le1,\\\frac14(2-t)^2,&1\le t\le2.\end{cases}
$$

The [Taylor expansion](taylor-expansion.md) with [integral](integral.md) remainder gives $L(f)=\int_0^2K(t)f^{(3)}(t)\,dt$, because $L$ annihilates [polynomials](polynomial-split.md) of degree at most two. Since $K\ge0$ and $\int_0^2K=1/3$, the sharp bound is $|L(f)|\le\frac13\|f^{(3)}\|_\infty$. Equality holds for $f(x)=x^3/6$.

## ↑ Ancestors (8)

1. [Sharp error constants for a Peano kernel](sharp-error-constants-for-a-peano-kernel.md)
2. [Peano kernel](peano-kernel.md)
3. [Peano kernel theorem](peano-kernel-theorem.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
