<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume an axisymmetric [thin disc](../../../../../../thin-disk.md) rotating in the fixed potential of a dominant central mass, with $\Omega=(GM_*)^{1/2}r^{-3/2}$ independent of time and height. Neglect vertical mass loss and vertical [angular-momentum flux](../../../../../../angular-momentum-flux.md) at the two faces, as well as [self-gravity](../../../../../../self-gravity.md) and radial [pressure](../../../../../../pressure.md) corrections to the rotation law. Define the [surface density](../../../../../../surface-density-of-a-disk.md) and density-weighted [kinematic viscosity](../../../../../../kinematic-viscosity.md) by

$$
\Sigma=\int\rho\,dz,\qquad \bar\nu=\frac1\Sigma\int\rho\nu\,dz,
$$

and let $v_r=\Sigma^{-1}\int\rho u_r\,dz$. These assumptions give the [vertically averaged viscous disk equations](../../../../../../vertically-averaged-viscous-disk-equations.md)

$$
\partial_t\Sigma+\frac1r\partial_r(r\Sigma v_r)=0,\qquad
\partial_t(\Sigma l)+\frac1r\partial_r(r\Sigma v_rl-r^3\bar\nu\Sigma\Omega')=0,
$$

where $l=r^2\Omega$ is [specific angular momentum](../../../../../../specific-angular-momentum.md). Subtract $l$ times [conservation of mass](../../../../../../mass-conservation.md) from [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md). Since $l$ is fixed in time,

$$
r\Sigma v_r l'=\partial_r(r^3\bar\nu\Sigma\Omega'),\qquad
v_r=-\frac3{\Sigma r^{1/2}}\partial_r(r^{1/2}\bar\nu\Sigma).
$$

Substitution into [conservation of mass](../../../../../../mass-conservation.md) proves the [Keplerian viscous diffusion equation](../../../../../../keplerian-viscous-diffusion-equation.md)

$$
\boxed{\partial_t\Sigma=\frac3r\partial_r\left[r^{1/2}\partial_r(r^{1/2}\bar\nu\Sigma)\right].}
$$

No assumption of height-independent [kinematic viscosity](../../../../../../kinematic-viscosity.md) is needed; its density-weighted average is the one appearing in the integrated stress. A wind or surface magnetic stress would add terms and must not be silently discarded.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
