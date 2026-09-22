<h1 id="d/d4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [function](../../../../../function-split.md) is nonnegative and [continuous](../../../../../continuous-function.md) on the positive quadrant. In [polar coordinates](../../../../../polar-coordinates.md) its product integral is, by the nonnegative [change of variables formula](../../../../../change-of-variables-formula.md) and [Tonelli's theorem](../../../../../tonelli-theorem.md),

$$
\int_0^{\pi/2}\int_0^\infty e^{-r^2}r^3(\cos\theta)^{3/2}(\sin\theta)^{1/2}\,dr\,d\theta.
$$

The angular factor is at most one, while the supplied radial integral is $1/2$, so the product integral is at most $\pi/4$ and is finite. This establishes integrability before any signed interchange is used.

Let $A$ denote the angular integral. The polar evaluation is $A/2$. In Cartesian coordinates [Fubini's theorem](../../../../../fubini-s-theorem.md) instead factors the integral as

$$
\left(\int_0^\infty e^{-x^2}x^{3/2}\,dx\right)
\left(\int_0^\infty e^{-y^2}y^{1/2}\,dy\right)
=\frac14\left(\int_0^\infty e^{-u}u^{1/4}\,du\right)
\left(\int_0^\infty e^{-v}v^{-1/4}\,dv\right),
$$

using $u=x^2$, $v=y^2$. All factors converge: their powers exceed $-1$ at zero and the exponential controls infinity. Equating the evaluations gives

$$
\boxed{A=\frac12\left(\int_0^\infty e^{-u}u^{1/4}\,du\right)\left(\int_0^\infty e^{-v}v^{-1/4}\,dv\right)}.
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
