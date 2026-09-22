<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Since the endpoints represent the same point of the tube, both density and diffusive flux must match. For a positive [diffusion](../../../../diffusion.md) coefficient $\lambda$, the [periodic boundary conditions](../../../../periodic-boundary-conditions.md) are

$$
\boxed{u(-\pi,t)=u(\pi,t),\qquad u_x(-\pi,t)=u_x(\pi,t).}
$$

For [separation of variables](../../../../separation-of-variables.md), periodic spatial modes solve $X''+n^2X=0$ and have time factors $e^{-\lambda n^2t}$. The constant mode has no decay. The [periodic diffusion on a circle](../../../../periodic-diffusion-on-a-circle.md) solution is therefore

$$
u(x,t)=\frac{a_0}{2}+\sum_{n=1}^\infty[a_n\cos(nx)+b_n\sin(nx)]e^{-\lambda n^2t},
$$

where the [Fourier coefficients](../../../../fourier-coefficient.md) are

$$
a_n=\frac1\pi\int_{-\pi}^\pi f(x)\cos(nx)dx,\qquad b_n=\frac1\pi\int_{-\pi}^\pi f(x)\sin(nx)dx.
$$

The expression for $a_n$ includes $n=0$.

The specified profile is even, so $b_n=0$. Its mean follows from $\int_0^\pi(\pi-x)^2dx=\pi^3/3$, giving $a_0=2\pi^2/3$. For $n\geq1$, two [integrations by parts](../../../../integration-by-parts.md) give

$$
\int_0^\pi(\pi-x)^2\cos(nx)dx=\frac{2\pi}{n^2},\qquad a_n=\frac4{n^2}.
$$

Consequently

$$
\boxed{u(x,t)=\frac{\pi^2}{3}+4\sum_{n=1}^\infty\frac{\cos(nx)}{n^2}e^{-\lambda n^2t}.}
$$

All nonconstant [normal modes](../../../../normal-mode.md) decay for $\lambda>0$, so the density becomes uniform:

$$
\boxed{u(x,t)\longrightarrow\frac{\pi^2}{3}\quad(t\to\infty).}
$$

The conserved total amount is $\int_{-\pi}^\pi u\,dx=2\pi^3/3$. The initial cusp at zero is compatible with an [L2 space](../../../../l2-space-is-a-hilbert-space.md) solution and is immediately smoothed by [diffusion](../../../../diffusion.md). At $\lambda=0$ there would be no relaxation, so positivity is needed for this long-time conclusion.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
