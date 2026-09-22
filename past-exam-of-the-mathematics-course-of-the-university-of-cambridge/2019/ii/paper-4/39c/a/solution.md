<h1 id="39c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Expand the unknown in [Fourier modes](../../../../../../fourier-mode.md):

$$
u(x)=\sum_{n\in\mathbb Z}\widehat u_n e^{i\pi nx}.
$$

By [Termwise differentiation of a Fourier series](../../../../../../termwise-differentiation-of-a-fourier-series.md),

$$
-\frac1{\pi^2}u''
=\sum_{n\in\mathbb Z}n^2\widehat u_n e^{i\pi nx}.
$$

Also,

$$
1+2\cos\pi x=1+e^{i\pi x}+e^{-i\pi x}.
$$

Therefore the coefficient of $e^{i\pi mx}$ on the left-hand side is

$$
(m-1)^2\widehat u_{m-1}
+(m^2+1)\widehat u_m
+(m+1)^2\widehat u_{m+1}.
$$

The right-hand side has coefficients

$$
\widehat f_m=\frac1{m^2+1},
\qquad m\in\mathbb Z,
$$

because the coefficient of each of $e^{\pm i\pi nx}$ is $1/(n^2+1)$ and the constant coefficient is one. Hence the [Fourier spectral system for a cosine-modulated second derivative](../../../../../../fourier-spectral-system-for-a-cosine-modulated-second-derivative.md) is

$$
\boxed{
(m-1)^2\widehat u_{m-1}
+(m^2+1)\widehat u_m
+(m+1)^2\widehat u_{m+1}
=\frac1{m^2+1},
\qquad m\in\mathbb Z.}
$$

Its coefficient array is an infinite [tridiagonal matrix](../../../../../../tridiagonal-matrix.md).

For a [spectral truncation](../../../../../../spectral-truncation.md), retain the modes $-M\leq n\leq M$, set

$$
\widehat u_{-M-1}=\widehat u_{M+1}=0,
$$

and impose the displayed coefficient equation for every $-M\leq m\leq M$. This gives an explicit $(2M+1)$-dimensional tridiagonal system. The resulting finite [Fourier series](../../../../../../fourier-series-split.md) automatically satisfies the periodic boundary conditions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
