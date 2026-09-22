<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The energy density from a [phase-space distribution function](../../../../../../phase-space-distribution-function.md) with $g=2$ internal states is

$$
\rho_\nu=\frac{g}{(2\pi)^3}
\int_{\mathbb R^3}\frac{\sqrt{p^2+m_\nu^2}}{e^{p/T_\nu}+1}\,d^3p
=\frac{g}{2\pi^2}\int_0^\infty
\frac{p^2\sqrt{p^2+m_\nu^2}}{e^{p/T_\nu}+1}\,dp.
$$

In the ultrarelativistic limit $T_\nu\gg m_\nu$, set $x=p/T_\nu$. The [Fermi-Dirac distribution](../../../../../../fermi-dirac-distribution.md) then gives

$$
\rho_\nu=\frac{T_\nu^4}{\pi^2}
\int_0^\infty\frac{x^3}{e^x+1}\,dx
=\frac{T_\nu^4}{\pi^2}
3!\left(1-2^{-3}\right)\zeta(4).
$$

Since $\zeta(4)=\pi^4/90$,

$$
\boxed{\rho_\nu=\frac{7\pi^2}{120}T_\nu^4}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
