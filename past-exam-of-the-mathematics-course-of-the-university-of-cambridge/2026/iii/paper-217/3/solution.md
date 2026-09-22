<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The spectral characterization of the [Reproducing-kernel Hilbert space of a stationary Gaussian process](../../../../../reproducing-kernel-hilbert-space-of-a-stationary-gaussian-process.md) says that its elements are precisely the functions whose Fourier transforms satisfy

$$
\lVert f\rVert_{\mathcal H_K}^2
=c\int_{\mathbb R}\frac{|\widehat f(u)|^2}{\widehat K(u)}\,du<\infty,
$$

with $c$ determined only by the [Fourier transform](../../../../../fourier-transform.md) convention. Here $\widehat K(u)=(1+u^2)^{-1}$, so

$$
\lVert f\rVert_{\mathcal H_K}^2
=c\int_{\mathbb R}(1+u^2)|\widehat f(u)|^2\,du.
$$

This is an equivalent norm for the [Sobolev space](../../../../../sobolev-space-split.md) $H^1(\mathbb R)$, and hence the RKHS equals $H^1(\mathbb R)$ as a set.

Since $\widehat K$ is integrable, $K$ is continuous and the process has a jointly measurable separable version. For every finite Borel measure $\nu$ on $\mathbb R$, [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
\mathbb E\lVert X\rVert_{L^2(\nu)}^2
=\int_{\mathbb R}\mathbb E|X(t)|^2\,d\nu(t)
=K(0)\nu(\mathbb R)<\infty.
$$

Thus $X\in L^2(\mathbb R,\nu)$ almost surely and is a Borel random variable there. Every continuous linear functional of $X$ is a centered normal random variable: approximate its $L^2(\nu)$ integral by finite linear combinations of process values and pass to the $L^2$ limit. Therefore the induced law is a [Gaussian Borel measure](../../../../../gaussian-measure.md) on $L^2(\mathbb R,\nu)$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
