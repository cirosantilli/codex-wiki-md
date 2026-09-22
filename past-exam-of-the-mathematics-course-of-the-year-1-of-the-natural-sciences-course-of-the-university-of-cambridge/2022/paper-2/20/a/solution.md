<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a separated nonzero solution $T=f(x)g(y)$, substitution and division by $fg$ gives

$$
a\frac{f'}f=\frac{g''}g=-\lambda^2.
$$

The homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) impose $g(0)=g(1)=0$. For a nonzero spatial factor, [integration by parts](../../../../../integration-by-parts.md) gives $\lambda^2\int_0^1g^2dy=\int_0^1(g')^2dy$, so the separation value is nonnegative. The zero value gives only a trivial linear $g$ under these boundary conditions. The nontrivial separated factors, for $a\ne0$, are therefore

$$
\boxed{g_n(y)=B_n\sin(n\pi y),\qquad
f_n(x)=A_n e^{-n^2\pi^2x/a},\qquad n=1,2,\ldots}.
$$

For the intended forward [diffusion equation](../../../../../diffusion-equation-split.md), assume $a>0$. The [superposition principle](../../../../../superposition-principle.md) gives a [Fourier sine series](../../../../../fourier-sine-series.md), whose coefficients must expand the initial ramp in the interior:

$$
b_n=2\int_0^1y\sin(n\pi y)dy=\frac{2(-1)^{n+1}}{n\pi}.
$$

Consequently the standard heat-flow solution is

$$
\boxed{T(x,y)=\frac2\pi\sum_{n=1}^\infty
\frac{(-1)^{n+1}}n\,e^{-n^2\pi^2x/a}\sin(n\pi y),\qquad a>0,\ x>0}.
$$

It satisfies both lateral [boundary conditions](../../../../../boundary-condition.md) for $x>0$, and tends to $y$ as $x\downarrow0$ for $0<y<1$, also converging to the ramp in the [L2 norm](../../../../../l2-norm.md). The exponential coefficient decay justifies differentiating the series for positive $x$.

There is a genuine incompatibility in the printed data: at $(0,1)$ the lateral condition demands zero while the initial condition demands one. Thus **no function satisfies every stated value at that corner**. The displayed series solves the usual consistent interpretation with initial data on $0<y<1$ and lateral data for $x>0$; it cannot be continuous at the upper initial corner. This discrepancy is present in the original PDF.

The sign of $a$ is also unstated. If $a=0$, the spatial equation with two zero endpoints forces $T=0$, incompatible with the ramp. If $a<0$, the separated Fourier coefficients grow like $e^{n^2\pi^2x/|a|}/n$ and fail to be square summable for every $x>0$; these data therefore have no forward solution in the standard [L2 space](../../../../../l2-space-is-a-hilbert-space.md) class. The positive-$a$ assumption is essential to the stated heat-flow interpretation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
