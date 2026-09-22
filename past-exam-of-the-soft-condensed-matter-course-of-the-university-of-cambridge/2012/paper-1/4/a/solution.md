<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [linear viscoelasticity](../../../../../linear-viscoelasticity.md), [stress](../../../../../stress.md) is a linear functional of past [strain](../../../../../strain.md) increments: scaling the deformation scales the response, and responses to small deformations add. For a time-translation-invariant material, [Boltzmann superposition](../../../../../boltzmann-superposition.md) writes $\sigma(t)=\int_{-\infty}^tG(t-s)\dot\epsilon(s)ds$, where $G$ is a [relaxation modulus](../../../../../relaxation-modulus.md). The material combines reversible storage with delayed or dissipative response; the description is restricted to small deformations about the chosen state.

The [Maxwell model](../../../../../linear-maxwell-fluid.md) places an elastic [spring](../../../../../spring.md) and viscous [dashpot](../../../../../dashpot.md) in series. They carry the same [shear stress](../../../../../shear-stress.md) $\sigma$, and their [shear strains](../../../../../shear-strain.md) add:

$$
\epsilon=\epsilon_e+\epsilon_v,\qquad
\epsilon_e=\frac\sigma{G_0},\qquad
\dot\epsilon_v=\frac\sigma\eta.
$$

Differentiating gives

$$
\boxed{\dot\epsilon=\frac{\dot\sigma}{G_0}+\frac\sigma\eta,\qquad\tau=\frac\eta{G_0}.}
$$

Here $\epsilon$ is dimensionless [shear strain](../../../../../shear-strain.md), $\sigma$ [shear stress](../../../../../shear-stress.md) in pascals, $G_0$ the [spring](../../../../../spring.md) [shear modulus](../../../../../shear-modulus.md), $\eta$ [dashpot](../../../../../dashpot.md) [viscosity](../../../../../dynamic-viscosity-split.md) in $\mathrm{Pa\,s}$, and $\tau$ the [relaxation time](../../../../../relaxation-time.md). The first term describes changing elastic [strain](../../../../../strain.md); the second is viscous flow. In this model the material flows at long [times](../../../../../time-in-physics.md) and has zero static [shear modulus](../../../../../shear-modulus.md).

## ↑ Ancestors (14)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
