<h1 id="12/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Height above the surface is $h=r-R$. Integrate the [density](../../../../../../density.md) over all exterior spherical shells:

$$
M=\int_R^\infty\int_0^\pi\int_0^{2\pi}
\rho_0e^{-(r-R)/h_0}r^2\sin\theta\,d\phi\,d\theta\,dr
=4\pi\rho_0\int_0^\infty(R+h)^2e^{-h/h_0}\,dh.
$$

Repeated [integration by parts](../../../../../../integration-by-parts.md), or the substitution $h=h_0s$, gives

$$
\int_0^\infty e^{-h/h_0}\,dh=h_0,\quad
\int_0^\infty he^{-h/h_0}\,dh=h_0^2,\quad
\int_0^\infty h^2e^{-h/h_0}\,dh=2h_0^3.
$$

Expand $(R+h)^2$ and use these moments to obtain the [mass of an exponential spherical atmosphere](../../../../../../mass-of-an-exponential-spherical-atmosphere.md):

$$
\boxed{M=4\pi\rho_0h_0(R^2+2Rh_0+2h_0^2)}.
$$

For $h_0\ll R$, the leading term is surface area $4\pi R^2$ times column mass $\rho_0h_0$; the other terms retain the finite-curvature corrections.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [12](../../../12.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
