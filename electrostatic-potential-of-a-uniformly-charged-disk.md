# Electrostatic potential of a uniformly charged disk

↑ **Parent:** [Coulomb potential energy](coulomb-potential-energy.md)

A thin disk of radius $a>0$ in $z=0$ carries uniform [surface charge density](surface-charge-density.md) $\sigma=Q/(\pi a^2)$. Summing the [Coulomb potential](coulomb-potential-energy.md) of concentric rings gives the displayed axis potential, with zero reference at infinity. Put $A=\sigma/(2\epsilon_0)$, use [spherical coordinates](spherical-coordinate-system.md) $z=r\cos\theta$, and let $P_2(t)=(3t^2-1)/2$. The near-center expansion, separately harmonic above and below the charged sheet, is

$$
\psi(r,\theta)=A\left[a-r|\cos\theta|+\frac{r^2}{2a}P_2(\cos\theta)+O(r^4/a^3)\right].
$$

The absolute value represents the jump in normal [electric field](electric-field-split.md) across the sheet; a single regular [solid harmonic](solid-harmonic.md) series cannot describe both half-spaces simultaneously. The constant and quadratic coefficients follow from the positive-axis Taylor series, and reflection symmetry supplies the other half-space. The far-field [multipole expansion](electric-multipole-expansion.md) is

$$
\psi(r,\theta)=\frac{Q}{4\pi\epsilon_0}\left[\frac1r-\frac{a^2}{4r^3}P_2(\cos\theta)+O(a^4/r^5)\right].
$$

The monopole is the total charge, the dipole vanishes by reflection symmetry, and the next term is the axisymmetric [electric quadrupole](electric-quadrupole.md). These expansions converge for $r<a$ within each source-free half-space and for $r>a$ in the exterior, respectively; at a point of the sheet their potentials have continuous limiting values but their normal derivatives differ.

## ↑ Ancestors (7)

1. [Coulomb potential energy](coulomb-potential-energy.md)
2. [Coulomb's law](coulomb-s-law.md)
3. [Electrostatics](electrostatics-split.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/2/solution.md)
