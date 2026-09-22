<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a finite-intensity [Poisson random measure](../../../../../../poisson-random-measure.md), [independence](../../../../../../independent-random-variables.md) of counts gives the exponential [characteristic function](../../../../../../characteristic-function.md) formula. Apply it to the cutoff construction from part (a), including the deterministic compensation, and pass to the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) limit of the small jumps. The compensated integrand is $O(y^2)$ at zero and bounded on the large-jump region, so its integral converges absolutely:

$$
\mathbb E e^{iuX_t}=\exp\left\{t\int_{\mathbb R\setminus\{0\}}\left(e^{iuy}-1-iuy\mathbf1_{\{|y|\leq1\}}\right)c|y|^{-2}dy\right\}.
$$

Symmetry makes the absolutely integrable imaginary part zero. Substituting $z=|u|y$ in the real part and using the specified normalization gives

$$
2ct\int_0^\infty\frac{\cos(uy)-1}{y^2}dy
=-2ct|u|\int_0^\infty\frac{1-\cos z}{z^2}dz=-t|u|.
$$

Thus **$\mathbb E e^{iuX_1}=e^{-|u|}$**, and this construction is the standard [Cauchy process](../../../../../../cauchy-process.md). To calculate the density, its integrable [characteristic function](../../../../../../characteristic-function.md) permits [Fourier inversion](../../../../../../fourier-inversion-theorem.md):

$$
f_{X_1}(x)=\frac1{2\pi}\int_{\mathbb R}e^{-|u|}e^{-iux}du
=\frac1\pi\operatorname{Re}\int_0^\infty e^{-(1+ix)u}du
=\boxed{\frac1{\pi(1+x^2)}}.
$$

This is the standard [Cauchy distribution](../../../../../../cauchy-distribution.md). The normalization also gives $c=1/\pi$: integration by parts turns $\int_0^\infty(1-\cos z)z^{-2}dz$ into $\int_0^\infty\sin z\,dz/z=\pi/2$. For completeness, with exponential damping the latter integral equals $\arctan(1/\eta)$, because its derivative in frequency $b$ is $\int_0^\infty e^{-\eta z}\cos(bz)dz=\eta/(\eta^2+b^2)$ and its value at $b=0$ is zero. Let $\eta\downarrow0$; integration by parts bounds the undamped and damped tails uniformly by a constant divided by the lower cutoff, justifying the limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
