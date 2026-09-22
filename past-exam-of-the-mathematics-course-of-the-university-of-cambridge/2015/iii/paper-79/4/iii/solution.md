<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The interior [potential-vorticity equation](../../../../../../potential-vorticity-evolution-equation.md) alone does not determine the frequency. Use the [rigid-boundary buoyancy condition for quasi-geostrophic waves](../../../../../../rigid-boundary-buoyancy-condition-for-quasi-geostrophic-waves.md). Linear adiabatic [buoyancy](../../../../../../buoyancy.md) conservation about the basic state gives

$$
(\partial_t+\bar U\partial_x)b'+M^2v'+N^2w'=0,
\qquad b'=f_0\psi'_z,\qquad v'=\psi'_x.
$$

At $z=0$, the [impermeability condition](../../../../../../no-penetration-boundary-condition.md) sets $w'=0$ and the basic velocity is zero. Therefore

$$
f_0\psi'_{zt}+M^2\psi'_x=0,
\qquad c\widehat\psi'(0)=S\widehat\psi(0).
$$

Substitution of $\widehat\psi'(0)=-m\widehat\psi(0)$ yields the [dispersion relation of a semi-infinite Eady edge wave](../../../../../../dispersion-relation-of-a-semi-infinite-eady-edge-wave.md)

$$
\boxed{c=-\frac{S}{m}=-\frac{M^2|f_0|}{f_0N\sqrt{k^2+l^2}},\qquad \omega=kc.}
$$

For $f_0>0$, this is $c=-M^2/[N\sqrt{k^2+l^2}]$. The sign is fixed by both the thermal-wind relation and the lower-boundary buoyancy budget.

The [steering height of a semi-infinite Eady edge wave](../../../../../../steering-height-of-a-semi-infinite-eady-edge-wave.md) is obtained by cancelling the phase-speed term against the basic advection in the wave-following frame:

$$
\bar U(z_c)-c=-Sz_c+\frac S m=0,
\qquad \boxed{z_c=\frac1m=\frac{|f_0|}{N\sqrt{k^2+l^2}}.}
$$

Thus the [phase velocity](../../../../../../phase-velocity.md) equals the basic thermal-wind velocity at one penetration depth. For nonzero $M$ they have the same sign in the laboratory frame. If “exactly opposes the thermal wind” is read literally as $c=-\bar U(z)$, it instead gives $z=-1/m$, outside the fluid: **there is no positive physical height with opposite laboratory velocities**. The positive height above is the physically meaningful [critical level](../../../../../../critical-level-of-a-shear-flow-wave.md), where the $-c$ and $\bar U$ contributions to the wave-frame material derivative oppose and cancel. This distinction resolves the ambiguous printed wording without reversing the derived wave speed. If $M=0$, the shear and $c$ vanish, so there is no distinguished steering height.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
