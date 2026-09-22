# Kinematic viscosity

↑ **Parent:** [Dynamic viscosity](dynamic-viscosity-split.md)

The [kinematic viscosity](kinematic-viscosity.md) is [dynamic viscosity](dynamic-viscosity-split.md) divided by [mass density](density.md):

$$
\nu=\frac\mu\rho,\qquad [\nu]=\mathrm{m^2\,s^{-1}}.
$$

It measures the rate at which viscous transport smooths differences in [velocity](velocity.md). For constant $\mu$ and $\rho$ in [incompressible flow](incompressible-flow.md), dividing the [Navier-Stokes equation](navier-stokes-equation.md) by [mass density](density.md) makes the viscous acceleration $\nu\nabla^2\mathbf u$, where $\nabla^2$ is the [Laplacian](laplacian.md). [David Tong, Fluid Mechanics, section 3.1.1, p. 61](https://www.damtp.cam.ac.uk/user/tong/fluids/fluids.pdf)

For example, stipulate two [Newtonian fluids](newtonian-fluid.md) with the same [dynamic viscosity](dynamic-viscosity-split.md) $0.10\,\mathrm{Pa\,s}$ but different [mass densities](density.md). In the same steady [Couette flow](couette-flow.md) as above, both have [shear stress](shear-stress.md) $2.0\,\mathrm{Pa}$, but

$$
\begin{aligned}
\rho_1&=1000\,\mathrm{kg\,m^{-3}},&\nu_1&=1.0\times10^{-4}\,\mathrm{m^2\,s^{-1}},\\
\rho_2&=500\,\mathrm{kg\,m^{-3}},&\nu_2&=2.0\times10^{-4}\,\mathrm{m^2\,s^{-1}}.
\end{aligned}
$$

The same [viscous stress](viscous-stress-tensor.md) transports [momentum](momentum-split.md) through less [mass](mass.md) in the second fluid, so its [velocity](velocity.md) responds faster to a given nonuniform viscous [force](force-split.md).

To see the [diffusion equation](diffusion-equation-split.md) directly, consider an unsteady parallel [velocity field](velocity-field.md) $\mathbf u=(u(y,t),0,0)$ with constant material coefficients and no streamwise [pressure gradient](pressure-gradient.md) or body [force](force-split.md). Its [convective acceleration](convective-acceleration.md) vanishes, and the [Navier-Stokes equation](navier-stokes-equation.md) reduces to

$$
\partial_tu=\nu\partial_y^2u.
$$

Balancing $u/t$ against $\nu u/h^2$ gives the [viscous diffusion time](viscous-diffusion-time.md) $t_\nu\sim h^2/\nu$. For the $1.0\,\mathrm{mm}$ gap, the two fluids have scales $0.010\,\mathrm s$ and $0.0050\,\mathrm s$. This is a characteristic scale, not an exact settling time. For example, a perturbation of the [Couette flow](couette-flow.md) profile satisfying zero perturbation [velocity](velocity.md) at both plates is

$$
\delta u(y,t)=V\sin\left(\frac{\pi y}{h}\right)
\exp\left(-\frac{\pi^2\nu t}{h^2}\right).
$$

Substituting verifies the [diffusion equation](diffusion-equation-split.md); its amplitude falls by a factor $e$ in $h^2/(\pi^2\nu)$. [Kinematic viscosity](kinematic-viscosity.md) is therefore useful for predicting how quickly a moving wall influences the interior, while [dynamic viscosity](dynamic-viscosity-split.md) gives the [shear stress](shear-stress.md) at a prescribed [shear rate](shear-rate.md).

**Table of contents**

- [Momentum diffusion](momentum-diffusion.md)
- [Density-weighted mean kinematic viscosity](density-weighted-mean-kinematic-viscosity.md)
- [Density-weighted viscosity of a disk](density-weighted-viscosity-of-a-disk.md)

## ↑ Ancestors (5)

1. [Dynamic viscosity](dynamic-viscosity-split.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (119)

- [Blasius boundary layer](blasius-boundary-layer.md)
- [Burgers' equation](burgers-equation.md)
- [Burgers vortex sheet](burgers-vortex-sheet.md)
- [Chandrasekhar number](chandrasekhar-number.md)
- [Compact self-similar disk with density-linear viscosity](compact-self-similar-disk-with-density-linear-viscosity.md)
- [Critical internal-wave reflection](critical-internal-wave-reflection.md)
- [Cubic-exponent decay of a nonaxisymmetric shearing wave](cubic-exponent-decay-of-a-nonaxisymmetric-shearing-wave.md)
- [Darcy thermal-time Rayleigh number](darcy-thermal-time-rayleigh-number.md)
- [Density-weighted mean kinematic viscosity](density-weighted-mean-kinematic-viscosity.md)
- [Dissipation range](dissipation-range.md)
- [Eddy viscosity](eddy-viscosity.md)
- [Effective viscosity defined by disk stress](effective-viscosity-defined-by-disk-stress.md)
- [Ekman layer](ekman-layer.md)
- [Energy cascade](energy-cascade.md)
- [Enstrophy](enstrophy.md)
- [Equal-diffusivity magnetorotational channel](equal-diffusivity-magnetorotational-channel.md)
- [Euler limit](euler-limit.md)
- [Excess dissipation of a Burgers vortex](excess-dissipation-of-a-burgers-vortex.md)
- [Formal viscous inspiral time in Schwarzschild spacetime](formal-viscous-inspiral-time-in-schwarzschild-spacetime.md)
- [Free viscous decay between parallel plates](free-viscous-decay-between-parallel-plates.md)
- [Hartmann number](hartmann-number.md)
- [Inertial-diffusive scalar range](inertial-diffusive-scalar-range.md)
- [Kinematic viscosity](kinematic-viscosity.md)
- [Kinetic energy flux of circular Poiseuille flow](kinetic-energy-flux-of-circular-poiseuille-flow.md)
- [Kolmogorov 1941 theory](kolmogorov-1941-theory.md)
- [Kolmogorov first similarity hypothesis](kolmogorov-first-similarity-hypothesis.md)
- [Kolmogorov length scale](kolmogorov-length-scale.md)
- [Kolmogorov second similarity hypothesis](kolmogorov-second-similarity-hypothesis.md)
- [Laminar flow](laminar-flow.md)
- [Linearized Boussinesq equations](linearized-boussinesq-equations.md)
- [Magnetic Prandtl number](magnetic-prandtl-number.md)
- [Magnetohydrodynamic momentum equation](magnetohydrodynamic-momentum-equation.md)
- [Momentum diffusion](momentum-diffusion.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2013/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017/2/b/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2021/section-b/6/b/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022/section-b/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-36/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-40/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-73/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-68/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-74/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-84/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-79/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-79/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-79/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-81/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-71/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-74/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-87/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-67/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-68/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-79/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73/1/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73/3/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-73/3/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-54/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-54/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-54/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-54/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-57/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-76/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-64/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-333/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-321/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-337/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1/5c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-321/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/38b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-321/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345/2/b/ii/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-b/b8/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2/section-b/b8/d/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-b/b9/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1/1/c/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1/2/a/solution.md)
- [Prandtl boundary-layer equation](prandtl-boundary-layer-equation.md)
- [Prandtl number](prandtl-number.md)
- [Reynolds number](reynolds-number.md)
- [Reynolds pipe-and-dye experiment](reynolds-pipe-and-dye-experiment.md)
- [Schmidt number (fluid mechanics)](schmidt-number-fluid-mechanics.md)
- [Square-root-radius diffusion transform](square-root-radius-diffusion-transform.md)
- [Steady circular Couette profile](steady-circular-couette-profile.md)
- [Stokes flow](stokes-flow-split.md)
- [Surface density of a steady photoevaporating disk](surface-density-of-a-steady-photoevaporating-disk.md)
- [Surface Ekman layer](surface-ekman-layer.md)
- [Taylor number](taylor-number.md)
- [Torque-dominated accretion disk](torque-dominated-accretion-disk.md)
- [Townsend-Betchov cascade cartoon](townsend-betchov-cascade-cartoon.md)
- [Turbulent dissipation anomaly](turbulent-dissipation-anomaly.md)
- [Unbuttressed Newtonian grounding-line stress](unbuttressed-newtonian-grounding-line-stress.md)
- [Vertically averaged alpha closure for a mixed-pressure layer](vertically-averaged-alpha-closure-for-a-mixed-pressure-layer.md)
- [Viscous attenuation of an internal gravity wave](viscous-attenuation-of-an-internal-gravity-wave.md)
- [Viscous attenuation of an internal-wave beam](viscous-attenuation-of-an-internal-wave-beam.md)
- [Viscous-convective scalar range](viscous-convective-scalar-range.md)
- [Viscous diffusion time](viscous-diffusion-time.md)
- [Viscous magnetic-relaxation energy identity](viscous-magnetic-relaxation-energy-identity.md)
- [Zeroth law of turbulence](zeroth-law-of-turbulence.md)
