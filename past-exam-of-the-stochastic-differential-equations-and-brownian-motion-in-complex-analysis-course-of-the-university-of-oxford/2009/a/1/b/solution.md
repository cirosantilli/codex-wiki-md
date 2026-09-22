<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\lambda>1$, use $x/\lambda\geq1$ on the tail:

$$
\int_\lambda^\infty e^{-x^2/2}\,dx
\leq\frac1\lambda\int_\lambda^\infty xe^{-x^2/2}\,dx
=\frac{e^{-\lambda^2/2}}\lambda
\leq e^{-\lambda^2/2}.
$$

This proves the requested [Gaussian tail bound](../../../../../gaussian-tail-bound.md).

**The subsequent printed maximum inequality is false as stated.** For $n=1$ its integrand never reaches one, and its right-hand side is

$$
\frac2{\sqrt{2\pi}}\int_0^\infty e^{-x^2/2}\,dx=1.
$$

But for two independent absolute standard normal variables, using their common distribution function $F(x)=2\Phi(x)-1$ and the [standard normal density](../../../../../standard-normal-density.md) $\varphi$,

$$
\mathbb E M_1
=4\int_0^\infty x(2\Phi(x)-1)\varphi(x)\,dx
=8\int_0^\infty\varphi(x)^2\,dx
=\frac2{\sqrt\pi}>1.
$$

The middle step is [integration by parts](../../../../../integration-by-parts.md) with $\varphi'=-x\varphi$. Thus no proof of the displayed source inequality can hold for all its stated indices.

The correct [tail integral formula for expectation](../../../../../tail-integral-formula-for-expectation.md) is

$$
\mathbb E M_n=\int_0^\infty
\left[1-(2\Phi(x)-1)^{2^n}\right]\,dx.
$$

A valid [union bound](../../../../../boole-s-inequality.md) gives

$$
\mathbb P(M_n>x)\leq
\min\left(1,\frac{2^{n+1}}{\sqrt{2\pi}}\int_x^\infty e^{-u^2/2}\,du\right).
$$

In particular, for $x>1$ this is at most $\min(1,C_ne^{-x^2/2})$, where $C_n=2^{n+1}/\sqrt{2\pi}$. This corrected estimate proves the intended summability in part (c), without silently replacing the source formula.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
