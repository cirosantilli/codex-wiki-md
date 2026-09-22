<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A rising parcel cools, lowering the [saturation pressure](../../../../vapor-pressure.md). Once its [water vapor](../../../../water-vapor.md) supply exceeds that value, [atmospheric supersaturation](../../../../atmospheric-supersaturation.md) develops. [Homogeneous nucleation](../../../../homogeneous-nucleation.md) of pure [water](../../../../water.md) is strongly inhibited at the small [atmospheric supersaturations](../../../../atmospheric-supersaturation.md) typical of [clouds](../../../../cloud.md); existing [aerosol](../../../../aerosol.md) particles provide [cloud condensation nuclei](../../../../cloud-condensation-nucleus.md). Their dry sizes and composition, together with the parcel's ascent rate, determine how many [cloud droplets](../../../../cloud-droplet.md) activate.

[Köhler theory](../../../../kohler-theory.md) combines the [Kelvin equation](../../../../kelvin-equation.md), which raises equilibrium [vapor pressure](../../../../vapor-pressure.md) over a curved surface, with [Raoult's law](../../../../raoult-s-law.md), which lowers it for a [chemical solution](../../../../solution-chemistry.md). In a dilute diameter convention, with dry diameter $D_d$ and wet diameter $D$,

$$
s_{\rm eq}(D)\simeq\frac{A_K}D-\frac{\kappa_hD_d^3}{D^3},\qquad
A_K=\frac{4\sigma_wM_w}{RT\rho_w},\qquad
s_c(D_d,\kappa_h)=\left(\frac{4A_K^3}{27\kappa_hD_d^3}\right)^{1/2}.
$$

Here $s=e_v/E(T)-1$ is [atmospheric supersaturation](../../../../atmospheric-supersaturation.md), $\sigma_w$ is [surface tension](../../../../surface-tension-split.md), and $\kappa_h$ measures [aerosol hygroscopicity](../../../../aerosol-hygroscopicity.md), not the dry-[adiabatic process](../../../../adiabatic-process.md) exponent. The maximum of the [Köhler curve](../../../../kohler-curve.md) is the [critical supersaturation](../../../../critical-supersaturation.md). Larger or more hygroscopic particles generally have lower thresholds. [Cloud-droplet activation](../../../../cloud-droplet-activation.md) requires overcoming that maximum; total [aerosol](../../../../aerosol.md) number is not the activated number.

Given an observed [aerosol](../../../../aerosol.md) [number size distribution](../../../../number-size-distribution.md) $n_j(D_d)=dN_j/d\ln D_d$ for composition classes $j$, first assign each class a hygroscopicity and compute its [critical supersaturation](../../../../critical-supersaturation.md). If the parcel reaches maximum [atmospheric supersaturation](../../../../atmospheric-supersaturation.md) $s_{\max}$, the equilibrium-threshold estimate is

$$
D_{d,\min,j}=\left(\frac{4A_K^3}{27\kappa_{h,j}s_{\max}^2}\right)^{1/3},\qquad
\boxed{N_{\rm act}=\sum_j\int_{D_{d,\min,j}}^\infty n_j(D_d)\,d\ln D_d.}
$$

For each fitted [lognormal distribution](../../../../log-normal-distribution.md), this is its upper-tail [integral](../../../../integral-split.md); it can be evaluated analytically with an [error function](../../../../error-function.md) or numerically from measured bins.

The value $s_{\max}$ must be calculated, not guessed from the [aerosol](../../../../aerosol.md) distribution alone. Prescribe parcel upward [velocity](../../../../velocity.md) $w$, initial [pressure](../../../../pressure-split.md), [temperature](../../../../temperature-split.md) and [humidity](../../../../humidity.md), then integrate expansion cooling, [latent heat](../../../../latent-heat.md) release, conservation of total [water](../../../../water.md), and diffusional [cloud droplet](../../../../cloud-droplet.md) growth. Schematically,

$$
\frac{ds}{dt}=a_s w-b_s\frac{dq_l}{dt},\qquad
\frac{d r_i^2}{dt}=2G\,[s-s_{{\rm eq},i}(r_i)],
$$

where $a_s,b_s>0$, $G$ includes [water vapor](../../../../water-vapor.md) [diffusion](../../../../diffusion.md) and [thermal conduction](../../../../thermal-conduction.md), and $q_l$ is liquid [mass fraction](../../../../mass-fraction.md). Rising motion produces [atmospheric supersaturation](../../../../atmospheric-supersaturation.md); growing particles consume it. Their competition selects the peak and which particles cross their activation barriers. Assume a well-mixed closed parcel, liquid [water](../../../../water.md), soluble spherical particles, specified mixing state, and negligible [collision-coalescence](../../../../collision-coalescence.md) and fallout during activation. Slow kinetic growth, weakly soluble particles or [entrainment](../../../../fluid-entrainment.md) require a more detailed treatment than the threshold [integral](../../../../integral-split.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
