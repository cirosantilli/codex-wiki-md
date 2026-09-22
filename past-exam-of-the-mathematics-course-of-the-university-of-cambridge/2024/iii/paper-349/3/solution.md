<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [galactic distribution function](../../../../../galactic-distribution-function.md) $f(\mathbf x,\mathbf v,t)$ is the stellar mass or number per six-dimensional [phase space](../../../../../phase-space.md) volume,

$$
dM=f(\mathbf x,\mathbf v,t)\,d^3x\,d^3v.
$$

Its velocity moments give the spatial density, mean velocity, and [velocity dispersion](../../../../../velocity-dispersion.md); integrating those quantities along the line of sight and weighting by luminosity produces surface-brightness and line-of-sight-velocity observables. A model is compared with data only after the same projection, selection function, and instrumental convolution have been applied.

[Jeans theorem](../../../../../jeans-theorem.md) states that every steady solution of the [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) depends on phase-space coordinates only through [integrals of motion](../../../../../integral-of-motion.md). Conversely, every nonnegative function of isolating integrals is a steady collisionless distribution function on the region where those integrals are defined.

For the stated [power law](../../../../../power-law.md) in [relative energy](../../../../../relative-energy.md), isotropy gives

$$
\rho(\Psi)=4\pi F\int_0^{\sqrt{2\Psi}}
\left(\Psi-\frac{v^2}{2}\right)^{n-3/2}v^2\,dv.
$$

With the requested [change of variables](../../../../../change-of-variables-formula.md) $v=\sqrt{2\Psi}\cos\theta$, the density becomes

$$
\rho=8\sqrt2\pi F\Psi^n
\int_0^{\pi/2}\sin^{2n-2}\theta\cos^2\theta\,d\theta
=2\sqrt2\pi^{3/2}F
\frac{\Gamma(n-1/2)}{\Gamma(n+1)}\Psi^n,
$$

where the last equality uses the [Beta function](../../../../../beta-function.md) and [Gamma function](../../../../../gamma-function.md). Thus

$$
\boxed{\rho\propto\Psi^n}
$$

for $n>1/2$.

The normalized second velocity moment is

$$
\overline{v^2}
=\frac{\int_0^{\sqrt{2\Psi}}v^4(\Psi-v^2/2)^{n-3/2}\,dv}
{\int_0^{\sqrt{2\Psi}}v^2(\Psi-v^2/2)^{n-3/2}\,dv}.
$$

The same substitution and the [Beta-function recurrence](../../../../../beta-function-recurrence.md) give

$$
\overline{v^2}
=2\Psi\frac{B(5/2,n-1/2)}{B(3/2,n-1/2)}
=\boxed{\frac{3\Psi}{n+1}}.
$$

**Consequently the one-dimensional isotropic [velocity dispersion](../../../../../velocity-dispersion.md) is $\sigma^2=\overline{v^2}/3=\Psi/(n+1)$, proving the required linear dependence on the [relative potential](../../../../../relative-potential.md).**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
