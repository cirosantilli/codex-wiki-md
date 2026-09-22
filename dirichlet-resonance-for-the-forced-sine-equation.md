# Dirichlet resonance for the forced sine equation

↑ **Parent:** [Green's function](green-s-function-split.md)

A continuous forcing gives the solution with [zero](zero-of-a-function.md) initial data $z(x)=-\int_0^x\sin(x-s)f(s)\,ds$. Every solution vanishing at [zero](zero-of-a-function.md) is $A\sin x+z(x)$. If $\sin L\ne0$, the remaining endpoint determines $A$ uniquely, with [Green's function](green-s-function-split.md)

$$
G_L(x,s)=\frac{\sin(\min\{x,s\})\sin(L-\max\{x,s\})}{\sin L}.
$$

Its first derivative has jump $-1$, the correct sign for $-y''-y=f$. If $L=m\pi$ with a positive integer $m$, solvability instead requires $\int_0^L f(s)\sin s\,ds=0$, and the coefficient $A$ is free. This is the [Fredholm alternative](fredholm-alternative.md) with a one-dimensional homogeneous kernel.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
