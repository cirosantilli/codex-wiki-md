<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $x=r\cos\theta$. The function $e^{ikx}$ solves the two-dimensional [Helmholtz equation](../../../../../helmholtz-equation.md), $(\nabla^2+k^2)e^{ikx}=0$. Expand its angular dependence as a [Fourier series](../../../../../fourier-series-split.md),

$$
e^{ikr\cos\theta}=\sum_{m\in\mathbb Z}F_m(r)e^{im\theta}.
$$

Substitution into the polar-coordinate [Laplacian](../../../../../laplacian.md),

$$
\nabla^2=\partial_r^2+\frac1r\partial_r+\frac1{r^2}\partial_\theta^2,
$$

gives

$$
r^2F_m''+rF_m'+(k^2r^2-m^2)F_m=0.
$$

With $\rho=kr$, this is the [Bessel differential equation](../../../../../bessel-differential-equation.md). Regularity of the original [plane wave](../../../../../plane-wave.md) at the origin excludes the singular second-kind solution. Thus $F_m(r)$ is a constant multiple of the regular first-kind function, and

$$
\boxed{e^{ikr\cos\theta}=\sum_{m\in\mathbb Z}a_mJ_m(kr)e^{im\theta}.}
$$

For integer negative orders, $J_{-m}=(-1)^mJ_m$, so this indexing still supplies the regular radial solution. The radial equation fixes the form of each term; the small-radius plane-wave expansion fixes its coefficient.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
