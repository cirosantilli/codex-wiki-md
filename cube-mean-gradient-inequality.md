# Cube mean-gradient inequality

↑ **Parent:** [Poincare-Wirtinger inequality](poincare-wirtinger-inequality.md)

For the cube $Q=(0,L)^n$ and $u\in H^1(Q)$,

$$
\|u\|_{L^2(Q)}^2
\leq |Q|u_Q^2+\frac n2L^2\|Du\|_{L^2(Q)}^2,
\qquad
u_Q=\frac1{|Q|}\int_Qu.
$$

This follows from the pairwise-difference identity

$$
\int_Q|u-u_Q|^2=\frac1{2|Q|}\int_Q\int_Q|u(x)-u(y)|^2\,dx\,dy
$$

and a coordinate-by-coordinate path from $x$ to $y$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) bounds the squared sum of its $n$ increments by $n$ times the sum of their squares, while the one-dimensional [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) bounds each integrated increment by $L^{n+2}\|D_i u\|_2^2$. Division by $2|Q|=2L^n$ gives the stated constant.

## ↑ Ancestors (8)

1. [Poincare-Wirtinger inequality](poincare-wirtinger-inequality.md)
2. [Poincaré inequality](poincare-inequality.md)
3. [Sobolev space](sobolev-space-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
