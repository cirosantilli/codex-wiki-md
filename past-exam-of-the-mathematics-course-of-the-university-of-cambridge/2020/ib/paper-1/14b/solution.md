<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

Expand $g$ in its [Fourier sine series](../../../../../fourier-sine-series.md)

$$
g(y)=\sum_{n=1}^{\infty}g_n\sin(k_ny),
\qquad
k_n=\frac{n\pi}{a},
\qquad
g_n=\frac2a\int_0^a g(y)\sin(k_ny)\,dy.
$$

By [separation of variables](../../../../../separation-of-variables.md), the decaying solution of [Laplace equation](../../../../../laplace-equation.md) in each half-strip has $n$th mode proportional to $e^{-k_n|x|}\sin(k_ny)$. Continuity at $x=0$ and integration of the equation across the [Dirac delta function](../../../../../dirac-delta-function.md) require the normal-derivative jump

$$
\phi_x(0^+,y)-\phi_x(0^-,y)=g(y).
$$

The jump of $C_ne^{-k_n|x|}$ is $-2k_nC_n$, so

$$
\boxed{\phi(x,y)=-\sum_{n=1}^{\infty}\frac{g_n}{2k_n}e^{-k_n|x|}\sin(k_ny)}.
$$

For $g(y)=\delta(y-c)$, its Fourier coefficients are

$$
g_n=\frac2a\sin\frac{n\pi c}{a}.
$$

Thus

$$
\phi(x,y)=-\frac1\pi\sum_{n=1}^{\infty}
\frac1n e^{-n\pi|x|/a}
\sin\frac{n\pi y}{a}\sin\frac{n\pi c}{a}.
$$

Translation in $x$ gives the [Dirichlet Green function for an infinite strip](../../../../../dirichlet-green-function-for-an-infinite-strip.md) with source $(b,c)$:

$$
\boxed{G(x,y;b,c)=-\frac1\pi\sum_{n=1}^{\infty}
\frac1n e^{-n\pi|x-b|/a}
\sin\frac{n\pi y}{a}\sin\frac{n\pi c}{a}}.
$$

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
