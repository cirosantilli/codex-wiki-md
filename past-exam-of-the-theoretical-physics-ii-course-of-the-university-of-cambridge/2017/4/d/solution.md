<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $m\geq0$, expand $e^{i\rho\cos\theta}=\exp[i\rho(e^{i\theta}+e^{-i\theta})/2]$. The lowest power producing the Fourier harmonic $e^{im\theta}$ is $(i\rho/2)^m/m!$. Meanwhile $J_m(\rho)\sim(\rho/2)^m/m!$. Matching these lowest powers gives $a_m=i^m$.

For negative order use $J_{-m}=(-1)^mJ_m$ and the equality of the positive and negative Fourier coefficients of this even function of $\theta$. This gives $a_{-m}=(-1)^mi^m=i^{-m}$. Therefore the [Jacobi-Anger expansion](../../../../jacobi-anger-expansion.md) is

$$
\boxed{e^{i\rho\cos\theta}=\sum_{m\in\mathbb Z}i^mJ_m(\rho)e^{im\theta}
=J_0(\rho)+2\sum_{m=1}^\infty i^mJ_m(\rho)\cos(m\theta).}
$$

The cosine form has multiplicity one for $m=0$ and two for every positive $m$. Those multiplicities are essential for matching the incident [plane wave](../../../../plane-wave.md).

## ↑ Ancestors (14)

1. [D](../d.md)
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
