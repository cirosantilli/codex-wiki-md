<h1 id="31b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the real [integral representation of the modified Bessel function of the second kind](../../../../../../integral-representation-of-the-modified-bessel-function-of-the-second-kind.md)

$$
K_\nu(x)=\frac12\int_{-\infty}^{\infty}\exp\{-x\cosh t+\nu t\}\,dt
=\frac12\int_{-\infty}^{\infty}e^{\nu h(t)}\,dt,
\qquad h(t)=t-\frac{x}{\nu}\cosh t.
$$

The unique [stationary point](../../../../../../stationary-point.md) is the strict maximum

$$
t_0=\operatorname{arsinh}\frac\nu x,
\qquad
\nu h(t_0)=\nu\operatorname{arsinh}\frac\nu x-\sqrt{\nu^2+x^2},
\qquad
\nu h''(t_0)=-\sqrt{\nu^2+x^2}.
$$

The [Laplace approximation](../../../../../../laplace-s-method.md) is consequently

$$
K_\nu(x)\sim
\frac12\left(\frac{2\pi}{\sqrt{\nu^2+x^2}}\right)^{1/2}
\exp\left\{\nu\operatorname{arsinh}\frac\nu x-\sqrt{\nu^2+x^2}\right\}.
$$

For fixed $x>0$, as $\nu\to+\infty$,

$$
\operatorname{arsinh}\frac\nu x=\log\frac{2\nu}{x}+O(\nu^{-2}),
\qquad
\sqrt{\nu^2+x^2}=\nu+O(\nu^{-1}).
$$

Substitution gives the required [large-order asymptotic of the modified Bessel function of the second kind](../../../../../../large-order-asymptotic-of-the-modified-bessel-function-of-the-second-kind.md):

$$
\boxed{K_\nu(x)\sim\left(\frac{\pi}{2\nu}\right)^{1/2}
\left(\frac{2\nu}{ex}\right)^\nu.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31B](../../31b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
