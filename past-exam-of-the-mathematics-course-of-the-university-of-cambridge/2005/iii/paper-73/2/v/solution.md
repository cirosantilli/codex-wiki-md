<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For axisymmetric disturbances, $k_y=0$, the [wavevector](../../../../../../wavevector.md) is fixed, so there is no winding/swing mechanism. Take $k_z\ne0$ and set $\chi=k_z^2/k^2$. Eliminating [pressure](../../../../../../pressure.md) with incompressibility gives

$$
\dot v_x=2\Omega\chi v_y-\nu k^2v_x,\qquad\dot v_y=-2(\Omega-A)v_x-\nu k^2v_y,\qquad v_z=-\frac{k_x}{k_z}v_x.
$$

The [axisymmetric incompressible epicyclic wave](../../../../../../axisymmetric-incompressible-epicyclic-wave.md) has inviscid frequency

$$
\omega^2=\kappa_r^2\chi,\qquad\kappa_r^2=4\Omega(\Omega-A),
$$

where $\kappa_r$ is the [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md).

In a Keplerian flow $A=3\Omega/4$ and $\kappa_r=\Omega$. The axisymmetric disturbances therefore execute stable inertial/epicyclic oscillations, with viscous [amplitude](../../../../../../wave-amplitude.md) decay $e^{-\nu k^2t}$. Rotation opposes sustained radial displacement through angular-momentum conservation. There can be bounded exchanges of [kinetic energy](../../../../../../kinetic-energy.md) between components, but no large Reynolds-number-dependent amplification of this axisymmetric family. Indeed, with $w=v_x/\sqrt\chi$, inviscid motion conserves

$$
(\Omega-A)|w|^2+\Omega|v_y|^2.
$$

Since the physical velocity norm is $|w|^2+|v_y|^2$, Keplerian [energy](../../../../../../energy.md) amplification is at most $\Omega/(\Omega-A)=4$; [viscosity](../../../../../../dynamic-viscosity.md) can only reduce that bound. A pure initial azimuthal disturbance can attain the inviscid factor four after a quarter epicyclic period. By contrast, the two-dimensional nonaxisymmetric [Orr mechanism](../../../../../../orr-mechanism.md) remains available in a Keplerian flow and has the $\mathrm{Re}^{2/3}$ gain derived above.

In non-rotating shear, $\Omega=0$ while $A$ remains nonzero. The axisymmetric solution is

$$
v_x=C_xe^{-\nu k^2\tau},\qquad v_y=(C_y+2A\tau C_x)e^{-\nu k^2\tau},\qquad\tau=t-t_0.
$$

Cross-stream motion transports the basic shear and generates an azimuthal streak: this is the [lift-up effect](../../../../../../lift-up-effect.md). Inviscid azimuthal velocity grows linearly and its [energy](../../../../../../energy.md) quadratically, rather than oscillating. With [viscosity](../../../../../../dynamic-viscosity.md), the gain for a suitable initial cross-stream disturbance scales as $[A/(\nu k^2)]^2$ at large [Reynolds number](../../../../../../reynolds-number.md), appreciably stronger than the two-dimensional $\mathrm{Re}^{2/3}$ scaling. For instance, $C_y=0$ and fixed $\chi>0$ give the leading optimized gain $4\chi A^2/(e^2\nu^2k^4)$ at $\tau\simeq1/(\nu k^2)$. Neither mechanism is an exponentially growing hydrodynamic [normal mode](../../../../../../normal-mode.md). **Rotation bounds axisymmetric lift-up in [Keplerian shear](../../../../../../keplerian-shear.md); without rotation, lift-up gives strong algebraic transient growth.** If $k_z=0$ as well as $k_y=0$, incompressibility forces $v_x=0$ and removes this coupling altogether.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
