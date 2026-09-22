<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Work in the small-slope model of a [transverse wave](../../../transverse-wave.md) on a taut string. Let $T$ be the constant [tension](../../../tension.md), $\rho$ the [linear mass density](../../../linear-mass-density.md), and take a right-moving sinusoidal [displacement](../../../displacement.md) $y=A\cos(\kappa x-\omega t)$, with [wave number](../../../wavenumber.md) $\kappa=\omega/v$. The [energy flux of a transverse string wave](../../../energy-flux-of-a-transverse-string-wave.md) through a cut is the transverse [force](../../../force-split.md) times transverse [velocity](../../../velocity.md):

$$
P(x,t)=-T\frac{\partial y}{\partial x}\frac{\partial y}{\partial t}
=T\kappa\omega A^2\sin^2(\kappa x-\omega t).
$$

A cycle average gives $\langle\sin^2\rangle=1/2$. Using $T=\rho v^2$, obtained from the string [wave equation](../../../wave-equation-split.md), yields

$$
\boxed{\overline P=\frac12T\kappa\omega A^2=\frac12\rho v\omega^2A^2.}
$$

The sign in the flux formula makes the [power](../../../power.md) positive for propagation in the positive $x$ direction.

The [energy](../../../energy-split.md) per unit equilibrium length is the sum of the kinetic and elastic terms:

$$
\mathcal E=\frac12\rho y_t^2+\frac12T y_x^2,
\qquad \langle\mathcal E\rangle=\frac12\rho\omega^2A^2.
$$

For a segment of [mass](../../../mass.md) $M=\rho\ell$ containing many [wavelengths](../../../wavelength.md), the spatial average agrees with the cycle average up to a small endpoint correction. Thus $E\simeq\tfrac12M\omega^2A^2$. Convert the given quantities to SI units: $M=0.080\ \mathrm{kg}$, $A=1.6\times10^{-4}\ \mathrm m$, and $\omega=2\pi(120)\ \mathrm{s}^{-1}$. Then

$$
\boxed{E\simeq\frac12(0.080)(240\pi)^2(1.6\times10^{-4})^2
=5.82\times10^{-4}\ \mathrm J.}
$$

The many-wavelength condition explains why no phase of the finite segment is needed. The result is exact as a cycle average, or for a segment containing an integer number of [wavelengths](../../../wavelength.md).

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
