<h1 id="section-b/4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [Kelvin-Voigt model](../../../../../kelvin-voigt-model.md) has no finite instantaneous elastic compliance: the viscous element prevents a sudden deformation under a finite [stress](../../../../../stress.md) step. Its [creep compliance](../../../../../creep-compliance.md) is

$$
J_K(t)=\frac1{G_0}\left(1-e^{-G_0t/\eta_0}\right),\qquad J_K(0^+)=0.
$$

Conversely an ideal [strain](../../../../../strain.md) step requires an impulsive [stress](../../../../../stress.md),

$$
\sigma(t)=\epsilon_0[G_0H(t)+\eta_0\delta(t)].
$$

After the impulse the held-strain response is simply constant. There is no finite stress-decay interval, and the [loss modulus](../../../../../loss-modulus.md) grows without bound as $\omega\to\infty$. This fails to represent a material with both a finite instantaneous stiffness and delayed [stress relaxation](../../../../../stress-relaxation.md).

The added series spring resolves this particular defect. At the instant of loading the Kelvin element cannot move but the added spring can. The [standard linear solid model](../../../../../standard-linear-solid-model.md) consequently has

$$
\boxed{G(t)=G_L+(G_H-G_L)e^{-t/\tau},\qquad t\geq0,}
$$

and

$$
\boxed{J(t)=\frac1{G_1}+\frac1{G_0}\left(1-e^{-G_0t/\eta_0}\right).}
$$

Its instantaneous stiffness is $G_H=G_1$, its long-time stiffness is $G_L$, and it exhibits genuine [stress relaxation](../../../../../stress-relaxation.md) as well as delayed creep. The creep retardation time $\eta_0/G_0$ differs from the stress-relaxation time $\tau=\eta_0/(G_0+G_1)$. These properties also follow directly from its constitutive equation,

$$
\eta_0\dot\sigma+(G_0+G_1)\sigma=G_1\eta_0\dot\epsilon+G_0G_1\epsilon.
$$

It remains an idealized solid with one relaxation mode: it cannot describe unrestricted long-time viscous flow, nonlinear response, or a broad spectrum of relaxation times.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
