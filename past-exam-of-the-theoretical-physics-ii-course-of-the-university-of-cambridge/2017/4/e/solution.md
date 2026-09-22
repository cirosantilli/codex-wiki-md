<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $w_0=1$ and $w_m=2$ for $m\geq1$, as required by the cosine form of the [Jacobi-Anger expansion](../../../../jacobi-anger-expansion.md). For a central real potential, the [Partial-wave S-matrix](../../../../partial-wave-s-matrix.md) is $S_m=e^{2i\delta_m}$. Splitting each shifted radial cosine into incoming and outgoing exponentials leaves its incoming coefficient unchanged and multiplies its outgoing coefficient by $S_m$. Subtracting the incident [plane wave](../../../../plane-wave.md) gives

$$
\psi_{\rm sc}\sim\frac{e^{ikr-i\pi/4}}{\sqrt{2\pi kr}}
\sum_{m=0}^\infty w_m(S_m-1)\cos(m\theta).
$$

Comparing with the prescribed [scattering amplitude](../../../../scattering-amplitude.md) convention yields the [two-dimensional partial-wave scattering formula](../../../../two-dimensional-partial-wave-scattering-formula.md),

$$
\boxed{f(\theta)=\frac1{i\sqrt{2\pi}}\sum_{m=0}^\infty w_m(e^{2i\delta_m}-1)\cos(m\theta)
=\sqrt{\frac2\pi}\sum_{m=0}^\infty w_me^{i\delta_m}\sin\delta_m\cos(m\theta).}
$$

[Orthogonality](../../../../orthogonal-vectors.md) gives $\int_0^{2\pi}1\,d\theta=2\pi$ and $\int_0^{2\pi}\cos^2(m\theta)d\theta=\pi$ for $m\geq1$, while all cross terms vanish. Hence

$$
\boxed{\lambda=\frac4k\left[\sin^2\delta_0+2\sum_{m=1}^\infty\sin^2\delta_m\right].}
$$

The multiplicities printed in this part are reversed. With those printed values and every $\delta_m=0$, the purported free wave would be $\tfrac12e^{ikr\cos\theta}+\tfrac32J_0(kr)$, rather than the required incident [plane wave](../../../../plane-wave.md). The extra $J_0$ contains an incoming cylindrical wave, which cannot be absorbed into $f$. The formulas above use the corrected multiplicities and therefore satisfy the specified scattering boundary condition.

## ↑ Ancestors (14)

1. [E](../e.md)
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
