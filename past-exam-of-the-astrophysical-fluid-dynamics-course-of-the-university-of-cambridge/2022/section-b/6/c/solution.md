<h1 id="section-b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use complex amplitudes and take their [real parts](../../../../../real-part.md) at the end. Write the radial surface displacement as $\eta=\epsilon e^{i(kz-\omega t)}$ and the combined potential as

$$
W=\epsilon\Pi_0I_0(kr)e^{i(kz-\omega t)}.
$$

The linear [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) is $u_r(R)=\partial_t\eta$. Differentiate it once more in time and use the radial momentum equation, $\partial_tu_r=-\partial_rW$, evaluated at the unperturbed radius $R$:

$$
\partial_t^2\eta=-\left.\partial_rW\right|_R.
$$

With $\kappa=kR$, the mode amplitudes therefore satisfy

$$
-\omega^2\epsilon=-\epsilon\Pi_0kI'_0(\kappa),
\qquad
\boxed{\Pi_0=\frac{\omega^2}{kI'_0(\kappa)}.}
$$

The prime differentiates the [Modified Bessel function of the first kind](../../../../../modified-bessel-function-of-the-first-kind.md) with respect to its dimensionless argument, rather than with respect to $r$. The result has units $\mathrm{m\,s^{-2}}$, as required because $\epsilon\Pi_0$ is a potential. It applies to $k>0$; the uniform $k=0$ limit requires separate treatment.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
