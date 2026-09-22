# Thermal diffusivity

↑ **Parent:** [Thermal conduction](thermal-conduction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_diffusivity)

[Thermal diffusivity](thermal-diffusivity.md) measures how rapidly [thermal conduction](thermal-conduction.md) smooths a [temperature](temperature-split.md) difference inside a material. [Thermal conductivity](thermal-conductivity.md) measures the [heat flux](heat-flux-density.md) driven by a specified [temperature gradient](temperature-gradient.md); [thermal diffusivity](thermal-diffusivity.md) also accounts for the [heat capacity](heat-capacity.md) that must be warmed. A material can carry substantial [heat](heat-split.md) yet change [temperature](temperature-split.md) slowly because it stores substantial [internal energy](internal-energy-split.md) per [kelvin](kelvin.md).

Write $\alpha=\kappa$ for [thermal diffusivity](thermal-diffusivity.md), reserving $k$ for [thermal conductivity](thermal-conductivity.md). In a homogeneous [isotropic](isotropy.md) material,

$$
\alpha=\frac{k}{\rho c}=\frac{k}{C_{\mathrm{vol}}},\qquad
[\alpha]=\frac{\mathrm{W\,m^{-1}\,K^{-1}}}{\mathrm{J\,m^{-3}\,K^{-1}}}
=\mathrm{m^2\,s^{-1}}.
$$

Here $\rho$ is [mass density](density.md), $c$ is [specific heat capacity](specific-heat-capacity.md) for the relevant mechanical constraint, and $C_{\mathrm{vol}}=\rho c$ is [volumetric heat capacity](volumetric-heat-capacity.md). The familiar $k/(\rho c_p)$ uses [specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md). For ordinary [solids](solid.md) with negligible thermal expansion, the difference between the two constrained [specific heat capacities](specific-heat-capacity.md) is often neglected. A rigid fixed-[volume](volume-thermodynamics.md) model instead uses [specific heat capacity at constant volume](specific-heat-capacity-at-constant-volume.md); a compressible moving [fluid](fluid.md) requires the accompanying [work](work.md) and transport terms. Thus the constraint is part of the approximation, not a choice made solely from the units. [NETZSCH, Principle of the LFA Method: conductivity equals diffusivity times specific heat capacity times density](light-and-laser-flash-analyzers-by-netzsch-analyzing-and-testing.md)

Assume a stationary material in the [continuum approximation](continuum-approximation.md), local thermal equilibration on times shorter than those resolved, no internal heating, no [phase transition](phase-transition.md), and negligible [convection](convection-split.md) and mechanical [work](work.md). Combining [conservation of energy](conservation-of-energy.md) with [Fourier's law](fourier-s-law.md) gives the one-dimensional balance

$$
\rho c\frac{\partial T}{\partial t}=-\frac{\partial q}{\partial x}
=\frac{\partial}{\partial x}\left(k\frac{\partial T}{\partial x}\right).
$$

If $k,\rho,c$ are constant over the region and [temperature](temperature-split.md) excursion, this becomes the [heat equation](heat-equation.md) $\partial_tT=\alpha\partial_x^2T$. If $k$ varies, retain the differentiated product; replacing it with $k\partial_x^2T$ loses a term. [Anisotropic](anisotropy.md) materials need a [thermal conductivity tensor](thermal-conductivity-tensor.md). The scalar constant-$\alpha$ examples below deliberately exclude these complications. [Carr, section 1: homogeneous isotropic constant-property assumptions; section 2, equations (1)–(3): insulated one-dimensional heat equation](rear-surface-integral-method-for-calculating-thermal-diffusivity-from-laser-flash-experiments-by-elliot-j-carr.md)

For an original comparison, stipulate two model materials with equal [thermal conductivity](thermal-conductivity.md) $k=2\,\mathrm{W\,m^{-1}\,K^{-1}}$ and equal [mass density](density.md) $\rho=1000\,\mathrm{kg\,m^{-3}}$, but [specific heat capacities](specific-heat-capacity.md) $c_A=1000$ and $c_B=4000\,\mathrm{J\,kg^{-1}\,K^{-1}}$. Then

$$
\alpha_A=2\times10^{-6}\,\mathrm{m^2\,s^{-1}},\qquad
\alpha_B=5\times10^{-7}\,\mathrm{m^2\,s^{-1}}.
$$

At the same [temperature gradient](temperature-gradient.md), both have the same instantaneous [heat flux](heat-flux-density.md) by [Fourier's law](fourier-s-law.md). At the same initial [temperature](temperature-split.md) profile and [boundary conditions](boundary-condition.md), material B takes four times as long to smooth a given spatial pattern. With fixed end [temperatures](temperature-split.md), identical geometry and no sources, both eventually have the same steady profile and [heat flux](heat-flux-density.md). The larger [heat capacity](heat-capacity.md) changes the transient, not this [steady state](steady-state.md). These are stipulated parameters, not measurements of named substances.

**Table of contents**

- [Ångström periodic heating method](angstrom-periodic-heating-method.md)
  - [Steady periodic thermal state](steady-periodic-thermal-state.md)
  - [Thermal diffusion wave](thermal-diffusion-wave.md)
    - [Thermal penetration depth](thermal-penetration-depth.md)
  - [Ångström method with linear heat loss](angstrom-method-with-linear-heat-loss.md)
  - [Ångström method worked example](angstrom-method-worked-example.md)
  - [Finite-end correction for periodic rod heating](finite-end-correction-for-periodic-rod-heating.md)
- [Prandtl number](prandtl-number.md)
- [Thermal diffusion time](thermal-diffusion-time.md)
  - [Thermal diffusion rate of a Fourier mode](thermal-diffusion-rate-of-a-fourier-mode.md)
  - [Thermal diffusion length](thermal-diffusion-length.md)
- [Laser flash analysis](laser-flash-analysis.md)

## ↑ Ancestors (7)

1. [Thermal conduction](thermal-conduction.md)
2. [Heat](heat-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (65)

- [Ångström method with linear heat loss](angstrom-method-with-linear-heat-loss.md)
- [Ångström method worked example](angstrom-method-worked-example.md)
- [Ångström periodic heating method](angstrom-periodic-heating-method.md)
- [Buoyancy displacement variable](buoyancy-displacement-variable.md)
- [Chandrasekhar number](chandrasekhar-number.md)
- [Darcy thermal-time Rayleigh number](darcy-thermal-time-rayleigh-number.md)
- [Diffusion](diffusion.md)
- [Finite-end correction for periodic rod heating](finite-end-correction-for-periodic-rod-heating.md)
- [Fourier analysis](fourier-analysis-split.md)
- [Fundamental diffusion mode](fundamental-diffusion-mode.md)
- [Half-space cooling model](half-space-cooling-model.md)
- [Laser flash analysis](laser-flash-analysis.md)
- [Magnetic-to-thermal diffusivity ratio](magnetic-to-thermal-diffusivity-ratio.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-43/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-73/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-84/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-84/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-75/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-74/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-67/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-80/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-80/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-77/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-77/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-65/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-71/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-76/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-78/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-337/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-332/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-338/1/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-332/2/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-1/10/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2/section-c/c12/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-c/c12/diffusion-with-a-heat-source/solution.md)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2013/paper-1/1/a/solution.md)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2015/paper-1/2/c/solution.md)
- [Prandtl number](prandtl-number.md)
- [Quasistatic temperature of a conductively cooled film](quasistatic-temperature-of-a-conductively-cooled-film.md)
- [Solutal diffusivity](solutal-diffusivity.md)
- [Strong Boussinesq approximation](strong-boussinesq-approximation.md)
- [Thermal conduction](thermal-conduction.md)
- [Thermal conductivity](thermal-conductivity.md)
- [Thermal diffusion length](thermal-diffusion-length.md)
- [Thermal-diffusion magnetic-field parameter](thermal-diffusion-magnetic-field-parameter.md)
- [Thermal diffusion rate of a Fourier mode](thermal-diffusion-rate-of-a-fourier-mode.md)
- [Thermal-diffusion scaling of a convection layer](thermal-diffusion-scaling-of-a-convection-layer.md)
- [Thermal diffusion time](thermal-diffusion-time.md)
- [Thermal diffusion wave](thermal-diffusion-wave.md)
- [Thermal diffusivity](thermal-diffusivity.md)
- [Thermosolutal convection](thermosolutal-convection.md)
- [Volumetric heat capacity](volumetric-heat-capacity.md)
