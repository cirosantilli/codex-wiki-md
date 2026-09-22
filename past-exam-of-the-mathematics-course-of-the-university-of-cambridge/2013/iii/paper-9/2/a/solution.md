<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention $\widehat\nu(\xi)=\int e^{-ix\cdot\xi}\,d\nu(x)$ throughout this question. The decay assumption implies square integrability, since [polar coordinates](../../../../../../polar-coordinates.md) give

$$
\int_{\mathbb R^2}|\widehat\mu(\xi)|^2\,d\xi
\lesssim\int_0^\infty\frac{r}{(1+r^{1+\epsilon})^2}\,dr<\infty.
$$

Near zero the integrand is bounded by $r$, and at infinity it is bounded by $r^{-1-2\epsilon}$. The positive $\epsilon$ is what makes the latter integrable.

By the [Plancherel theorem](../../../../../../plancherel-theorem.md), there is a function $g\in L^2(\mathbb R^2)$ whose [Fourier transform](../../../../../../fourier-transform.md) is $\widehat\mu$. It is the density of $\mu$ with respect to [Lebesgue measure](../../../../../../lebesgue-measure.md). To justify this step rather than assume a density, for every [Schwartz function](../../../../../../schwartz-function.md) $\varphi$, [Fourier inversion](../../../../../../fourier-inversion-theorem.md) gives

$$
\int\varphi\,d\mu
=(2\pi)^{-2}\int\widehat\varphi(-\xi)\widehat\mu(\xi)\,d\xi
=\int\varphi(x)g(x)\,dx.
$$

The [finite measure](../../../../../../finite-measure.md) and the locally integrable function thus define the same [tempered distribution](../../../../../../tempered-distribution.md), so they agree as measures: $d\mu=g\,dx$. In particular $g\ge0$ almost everywhere and $\int g=\mu(\mathbb R^2)<\infty$. This is the [L2 density from a square-integrable Fourier transform](../../../../../../l2-density-from-a-square-integrable-fourier-transform.md) principle.

For $f\in L^\infty(\mu)$, the density of $f\,d\mu$ is $fg$. The inequality $|f|\le\|f\|_{L^\infty(\mu)}$ holds wherever $g>0$, apart from a [Lebesgue measure](../../../../../../lebesgue-measure.md) zero set, so

$$
\|fg\|_2\le\|f\|_{L^\infty(\mu)}\|g\|_2.
$$

A second application of the [Plancherel theorem](../../../../../../plancherel-theorem.md) yields the explicit bound

$$
\boxed{\|\widehat{f\,d\mu}\|_2
=(2\pi)\|fg\|_2
\le\|\widehat\mu\|_2\,\|f\|_{L^\infty(\mu)}.}
$$

The implicit constant in the requested estimate may depend on the measure and its Fourier-decay bound, but is independent of $f$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
