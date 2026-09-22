<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Part (i) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) show

$$
\langle f,g\rangle=\lim_{N\to\infty}\langle S_Nf,g\rangle.
$$

Direct integration of this finite [Fourier partial sum](../../../../../../fourier-partial-sum.md) gives

$$
\langle S_Nf,g\rangle
=\sum_{|n|\leq N}\widehat f(n)\overline{\widehat g(n)}.
$$

Moreover [Bessel's inequality](../../../../../../bessel-s-inequality.md) puts both coefficient sequences in $\ell^2$, so their product series is absolutely convergent by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Consequently the cross form of [Parseval's identity](../../../../../../parseval-identity.md) is

$$
\boxed{\frac1{2\pi}\int_{-\pi}^{\pi}f(t)\overline{g(t)}\,dt
=\sum_{n\in\mathbb Z}\widehat f(n)\overline{\widehat g(n)}.}
$$

Taking $g=f$ also gives equality of the squared function norm and the squared coefficient norm.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
