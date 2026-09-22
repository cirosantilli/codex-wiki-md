<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

With the stated [Fourier transform](../../../../fourier-transform-split.md) convention, the [inverse Fourier transform](../../../../inverse-fourier-transform.md) and the deterministic [autocorrelation of a square-integrable function](../../../../autocorrelation-of-a-square-integrable-function.md) are

$$
\boxed{f(x)=\frac1{2\pi}\int_{\mathbb R}\widetilde f(k)e^{ikx}dk,\qquad h(x)=\int_{\mathbb R}\overline{f(y)}f(x+y)dy.}
$$

Assume initially sufficient decay and smoothness, for example a [Schwartz function](../../../../schwartz-function.md), to justify interchanging integrations and [Fourier inversion](../../../../fourier-inversion-theorem.md). With $s=x+y$, the [cross-correlation](../../../../cross-correlation.md) identity is

$$
\begin{aligned}
\widetilde h(k)&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikx}\overline{f(y)}f(x+y)dy\,dx\\
&=\left[\int_{\mathbb R}e^{iky}\overline{f(y)}dy\right]\left[\int_{\mathbb R}e^{-iks}f(s)ds\right]=|\widetilde f(k)|^2.
\end{aligned}
$$

Evaluating $h$ directly and by its inverse transform at zero proves the [Parseval identity](../../../../parseval-identity.md):

$$
\boxed{\int_{\mathbb R}|f(x)|^2dx=h(0)=\frac1{2\pi}\int_{\mathbb R}|\widetilde f(k)|^2dk.}
$$

Approximation extends the identity to [L2 space](../../../../l2-space-is-a-hilbert-space.md), as the [Plancherel theorem](../../../../plancherel-theorem.md).

For the compact cosine profile, the [Fourier transform of a truncated cosine](../../../../fourier-transform-of-a-truncated-cosine.md) follows from $\cos x=(e^{ix}+e^{-ix})/2$:

$$
\begin{aligned}
\widetilde f(k)&=\frac{\sin[(k-1)\pi/2]}{k-1}+\frac{\sin[(k+1)\pi/2]}{k+1}\\
&=\boxed{\frac{2\cos(k\pi/2)}{1-k^2}}.
\end{aligned}
$$

At $k=\pm1$ the apparent singularities are removable, with value $\pi/2$. The direct squared norm is $\int_{-\pi/2}^{\pi/2}\cos^2x\,dx=\pi/2$. Hence [Parseval identity](../../../../parseval-identity.md) and evenness give

$$
\int_0^\infty\frac{\cos^2(k\pi/2)}{(1-k^2)^2}dk=\frac{\pi^2}{8}.
$$

Putting $t=\pi k/2$ makes the left side $\pi^3/8$ times the requested integral. Therefore

$$
\boxed{\int_0^\infty\frac{\cos^2t}{(\pi^2/4-t^2)^2}dt=\frac1\pi.}
$$

At $t=\pi/2$ the integrand's continuous extension is $1/\pi^2$, so no principal-value prescription is required.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
