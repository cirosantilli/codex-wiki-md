<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $K=k_{\max}r$. Using the transform in part (a), the [band-limited linear density correlation](../../../../../../band-limited-linear-density-correlation.md) is

$$
\xi(r)=\frac{A}{2\pi^2r}\int_0^{k_{\max}}k^2\sin(kr)\,dk.
$$

Two integrations by parts give the antiderivative $-k^2\cos(kr)/r+2k\sin(kr)/r^2+2\cos(kr)/r^3$. Subtract its value at zero to obtain, for $r>0$,

$$
\boxed{\xi(r)=\frac{A}{2\pi^2r^4}\left[-K^2\cos K+2K\sin K+2(\cos K-1)\right].}
$$

The origin is a removable limit. The bracket starts with $K^4/4$, so

$$
\boxed{\xi(0)=\frac{Ak_{\max}^4}{8\pi^2}.}
$$

This is also the density variance obtained directly by setting $\sin(kr)/(kr)=1$ in the integral. The sharp spectral edge produces oscillatory correlations, with leading large-$r$ term $-Ak_{\max}^2\cos(k_{\max}r)/(2\pi^2r^2)$. A negative correlation at some separation is compatible with a nonnegative power spectrum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
