<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The incident [plane wave](../../../../plane-wave.md) is periodic in $\theta$, so expand it as a [Fourier series](../../../../fourier-series-split.md) $\sum_m R_m(r)e^{im\theta}$. Substitution into the [Helmholtz equation](../../../../helmholtz-equation.md), with $\rho=kr$, gives the radial [Bessel differential equation](../../../../bessel-differential-equation.md)

$$
\rho^2R_m''+\rho R_m'+(\rho^2-m^2)R_m=0.
$$

Regularity at the origin selects the [Bessel function of the first kind](../../../../bessel-function-of-the-first-kind.md), rather than the singular second solution. Thus

$$
\boxed{e^{ikr\cos\theta}=\sum_{m=-\infty}^\infty a_mJ_m(kr)e^{im\theta}.}
$$

The coefficients $a_m$ are independent of $r$; their values follow from matching near the origin in the next part. The completed identity is the [Jacobi-Anger expansion](../../../../jacobi-anger-expansion.md).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
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
