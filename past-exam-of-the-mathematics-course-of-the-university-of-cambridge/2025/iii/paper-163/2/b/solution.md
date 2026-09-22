<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The spacetime Fourier support of $g$ lies where $|\xi|\lesssim N$ and $|\tau|\lesssim N^2$. Choose a Schwartz function $\psi$ equal to one on this support and write $g=g*K_N$, where

$$
K_N(x,t)=N^4\check\psi(Nx,N^2t).
$$

This anisotropic reproducing kernel is the quantitative [local constancy principle](../../../../../../local-constancy-principle.md). Its Schwartz decay gives, for every $M$,

$$
|K_N(x,t)|\leq C_MN^4(1+N|x|+N^2|t|)^{-M}.
$$

Split the convolution at $(x_0,t_0)$ into the stated box $B$ and its complement. On $B$ the kernel is at most $C_0N^4$. Outside $B$, choosing $M$ in terms of $\epsilon$ makes its $L^1$ tail at most $C_\epsilon N^{-1000}$. Therefore

$$
\boxed{|g(x_0,t_0)|
\leq C_0N^4\int_B|g(x,t)|\,dxdt
+C_\epsilon N^{-1000}\|g\|_\infty.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 163](../../../paper-163-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
