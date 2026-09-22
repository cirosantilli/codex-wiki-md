<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\tau=t-t'$, $y=x-x'$ and $G(y,\tau)=(4\pi D\tau)^{-1/2}e^{-y^2/(4D\tau)}$ for $\tau>0$, with $D>0$. Direct differentiation gives

$$
\partial_\tau G=\left(-\frac1{2\tau}+\frac{y^2}{4D\tau^2}\right)G
=D\partial_y^2G.
$$

Also $\int_{\mathbb R}G\,dy=1$ and, for a smooth bounded [test function](../../../../../test-function.md) $f$,

$$
\int_{\mathbb R}G(y,\tau)f(y)\,dy
=\frac1{\sqrt\pi}\int_{\mathbb R}e^{-u^2}f(\sqrt{4D\tau}\,u)\,du
\longrightarrow f(0).
$$

Thus $G(\cdot,\tau)$ tends to a [Dirac delta distribution](../../../../../dirac-delta-function.md) as $\tau\downarrow0$. Defining the retarded kernel $K=\Theta(\tau)G$ supplies the initial impulse:

$$
\boxed{(\partial_t-D\partial_x^2)K
=\delta(t-t')\delta(x-x'),\qquad K=0\text{ for }t<t'.}
$$

The source term arises from the jump at $\tau=0$ in the distributional sense; differentiating only the smooth positive-time Gaussian would miss it.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
