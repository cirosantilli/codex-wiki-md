<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\Sigma=\Sigma_0x^{-5/2}g$ because the prescribed [kinematic viscosity](../../../../../../../kinematic-viscosity.md) is $\bar\nu=\bar\nu_0x^{5/2}$. Substituting $r=r_0x$ and $\partial_t=(3\bar\nu_0/4r_0^2)\partial_\tau$ into the [viscous evolution of an accretion disk](../../../../../../../viscous-evolution-of-an-accretion-disk.md) gives

$$
x^{-5/2}g_\tau=\frac4x\partial_x\left[x^{1/2}\partial_x(x^{1/2}g)\right].
$$

Hence the dimensionless [diffusion equation](../../../../../../../diffusion-equation-split.md) is

$$
\boxed{g_\tau=4x^{5/2}g_{xx}+6x^{3/2}g_x.}
$$

For the useful inverse-radius coordinate $y=x^{-1/2}$, this becomes simply $g_\tau=y g_{yy}$. The positive factor in $\tau=1+3\bar\nu_0t/(4r_0^2)$ makes increasing $\tau$ correspond to increasing physical time.

There is a distinction between the named torque variable and the physical [viscous torque in an accretion disk](../../../../../../../viscous-torque-in-an-accretion-disk.md). For [Keplerian rotation](../../../../../../../keplerian-disk.md), the outward torque magnitude is

$$
\mathcal T=3\pi\bar\nu\Sigma\sqrt{GM_\star r}=3\pi\bar\nu_0\Sigma_0\sqrt{GM_\star r_0}\,x^{1/2}g.
$$

Here $M_\star$ denotes the central [mass](../../../../../../../mass.md). The [zero-torque inner boundary condition](../../../../../../../zero-torque-inner-boundary-condition.md) therefore requires $x^{1/2}g\to0$ as $x\to0$. Requiring $g\to0$ is stronger. The nontrivial finite-mass profile used below satisfies both; this distinction matters when counting integration constants.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
