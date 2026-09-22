<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [first Born approximation](../../../../born-approximation.md), with incident and outgoing wave vectors $\mathbf k,\mathbf k'$, put $\mathbf q=\mathbf k'-\mathbf k$. For elastic scattering,

$$
q=2k\sin\frac\theta2,
\qquad f_B=-\frac{m}{2\pi\hbar^2}\int e^{-i\mathbf q\cdot\mathbf r}V(r)\,d^3r.
$$

Choose the polar axis along $\mathbf q$. The angular integral is

$$
\int e^{-iqr\cos\vartheta}\,d\Omega
=2\pi\int_{-1}^1e^{-iqru}\,du=4\pi\frac{\sin(qr)}{qr}.
$$

The radial [Dirac delta distribution](../../../../dirac-delta-function.md) then gives

$$
f_B=-\frac{2mV_0}{\hbar^2}\int_0^\infty r^2\delta(r-R)\frac{\sin(qr)}{qr}\,dr.
$$

Thus, introducing the [dimensionless](../../../../dimensionless-quantity.md) shell strength $g=2mV_0R/\hbar^2$,

$$
\boxed{f_B(\theta)=-\frac{2mV_0R}{\hbar^2q}\sin(qR)
=-gR\frac{\sin(qR)}{qR}}.
$$

The forward value is the continuous limit $f_B(0)=-gR$. This is the [delta-shell Born amplitude](../../../../delta-shell-born-amplitude.md), with its angular dependence expressed through the [momentum transfer](../../../../momentum-transfer.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
