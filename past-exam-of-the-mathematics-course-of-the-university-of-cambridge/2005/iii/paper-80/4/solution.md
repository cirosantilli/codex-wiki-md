<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Stable stratification is a constraint on motion, not an isolated parcel spring.** A light-over-heavy [density](../../../../../density.md) profile has $N^2=-(g/\rho_0)\bar\rho_z>0$. An adiabatically displaced parcel has [buoyancy](../../../../../buoyancy.md) anomaly $b=-N^2\xi_z$ relative to its surroundings. If one neglects the [pressure](../../../../../pressure.md) response and movement of surrounding fluid, the vertical equation would be $\ddot\xi_z=-N^2\xi_z$. A finite spherical blob cannot satisfy that isolated-oscillator picture: [incompressible flow](../../../../../incompressible-flow.md) requires surrounding fluid motion, and the [pressure](../../../../../pressure.md) perturbation communicates its acceleration to the rest of the fluid.

This can be shown directly with the linear [Boussinesq equations](../../../../../boussinesq-equations.md). For a uniform background, take a Fourier wavevector $(\mathbf k_h,m)$. [Pressure](../../../../../pressure.md) removes the component of the [buoyancy](../../../../../buoyancy.md) force parallel to this wavevector. Taking the divergence of momentum to determine [pressure](../../../../../pressure.md) and projecting the vertical component gives

$$
w_t=\frac{k_h^2}{k_h^2+m^2}b,\qquad b_t=-N^2w,
$$

so

$$
\boxed{\omega^2=N^2\frac{k_h^2}{k_h^2+m^2}.}
$$

This [pressure projection in a displaced stratified blob](../../../../../pressure-projection-in-a-displaced-stratified-blob.md) produces frequencies less than $N$ except for wavevectors with $m=0$. A localized spherical perturbation contains a range of directions and therefore a range of frequencies. It deforms and emits [internal gravity waves](../../../../../internal-wave.md), rather than remaining one sphere oscillating coherently at $N$. The [added mass](../../../../../added-mass.md) of a rigid sphere is a useful inertia analogy, but its numerical correction does not define an exact oscillation frequency for a deformable material blob in stratified fluid.

**Internal waves and energy transport.** The restoring force supports anisotropic [internal gravity waves](../../../../../internal-wave.md): their frequency depends on the direction, not just the length, of the wavevector. For a two-dimensional positive-frequency branch, $\omega=Nk/\sqrt{k^2+m^2}$ with $k>0$. Differentiation gives

$$
c_{gx}=\frac{Nm^2}{(k^2+m^2)^{3/2}},\qquad
c_{gz}=-\frac{Nkm}{(k^2+m^2)^{3/2}}.
$$

The vertical group and phase velocities have opposite signs. Wave energy therefore travels along a direction different from the direction of phase propagation, a point essential in selecting radiation conditions for wave-generating obstacles.

For constant $N$, the linear perturbation energy [density](../../../../../density.md) per reference mass is

$$
\mathcal E=\frac12|\mathbf u|^2+\frac{b^2}{2N^2}.
$$

Dot momentum with velocity and multiply [buoyancy](../../../../../buoyancy.md) evolution by $b/N^2$; the $bw$ terms cancel, leaving $\partial_t\mathcal E+\nabla\cdot(\Pi\mathbf u)=0$. The second term is the available potential energy stored by displacement against the stable [density](../../../../../density.md) profile. In an ideal fluid, that energy is exchanged with kinetic energy or transported away, not irreversibly dissipated by [buoyancy](../../../../../buoyancy.md) diffusion.

**Steady flows, layers and topography.** Stable stratification penalizes vertical displacement and favors flows with small vertical motion when the stratified [Froude number](../../../../../froude-number.md) $U/(NH)$ is small. The natural vertical displacement scale associated with kinetic energy $U^2$ is of order $U/N$; obstacles requiring much larger displacements can cause blocking and diversion instead of simple overpassing. In the ideal model fluid retains its [buoyancy](../../../../../buoyancy.md) label, so motion tends to follow [density](../../../../../density.md) surfaces. This inhibits vertical mixing but does not forbid horizontal rearrangement or turbulence powered by a shear flow.

A uniform current crossing topography generates stationary internal waves when its intrinsic frequency lies in the internal-wave range. For horizontal [wavenumber](../../../../../wavenumber.md) $k$, stationarity gives $m^2=N^2/U^2-k^2$. Height-dependent wind and stratification replace this by the [Scorer parameter](../../../../../scorer-parameter.md) relation derived in Question 1. A decrease of that parameter can produce a turning level, evanescence and vertical trapping, explaining lee-wave trains confined near a lower boundary. The exact channel superpositions in Question 1 also show that nonlinearity does not automatically destroy every wave solution.

Stability of the background [density](../../../../../density.md) profile does not imply stability of every flow built on it. Sufficiently large waves can overturn [density](../../../../../density.md) surfaces, and shear can supply energy to disturbances. Ideal advection can create fine structure, but irreversible homogenization of [buoyancy](../../../../../buoyancy.md) in a real fluid additionally involves diffusion or dissipation. A finite-amplitude ideal solution is consequently distinct from a guaranteed stable or physically realizable state.

**How rotation changes the picture.** With the vertical Coriolis parameter $f$, the corresponding uniform-background inertia–gravity dispersion becomes

$$
\omega^2=\frac{N^2k_h^2+f^2m^2}{k_h^2+m^2}.
$$

When $N>|f|$, the propagating branch lies between $|f|$ and $N$. Rotation also allows a slow balanced sector: horizontal [pressure](../../../../../pressure.md) and Coriolis forces balance, vertical [pressure](../../../../../pressure.md) and [buoyancy](../../../../../buoyancy.md) balance, and the circulation can be described through [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md). Small [Rossby number](../../../../../rossby-number.md) and small stratified Froude number lead to the quasi-geostrophic equations rather than to the fast internal-wave dynamics. Vertical shear is then tied to horizontal [buoyancy](../../../../../buoyancy.md) gradients through thermal-wind balance.

In this balanced sector, a planetary or topographic PV gradient supports [Rossby waves](../../../../../rossby-wave.md), whose restoring mechanism is conservation of PV under displacement across that gradient. Stable stratification couples horizontal levels through the $\partial_z[(f_0^2/N^2)\psi_z]$ term, and the mountain-wave calculation in Question 3 illustrates its vertical propagation filter. Thus stratification can support rapid buoyancy-restored waves, constrain slowly evolving balanced circulation, and shape interactions with boundaries; which description applies depends on the velocity, length, time and rotation scales.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
