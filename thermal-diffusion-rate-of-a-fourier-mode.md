# Thermal diffusion rate of a Fourier mode

↑ **Parent:** [Thermal diffusion time](thermal-diffusion-time.md)

With [thermal diffusivity](thermal-diffusivity.md) $\xi$, a [Fourier mode](fourier-mode.md) of angular [wavenumber](wavenumber.md) $k$ decays at rate $\beta=\xi k^2$. To avoid confusing this $k$ with [thermal conductivity](thermal-conductivity.md), use $\alpha=\xi$ and angular [wavenumber](wavenumber.md) $K$ below: the same rate is $\beta=\alpha K^2$, with units $\mathrm{s^{-1}}$.

Consider an insulated bar $0\leq x\leq L$ with constant [thermal diffusivity](thermal-diffusivity.md), no sources and no [heat flux](heat-flux-density.md) through either end or the sides. An original initial [temperature](temperature-split.md) profile and its exact evolution are

$$
T(x,0)=\overline T+A_0\cos\frac{n\pi x}{L},\qquad
T(x,t)=\overline T+A_0e^{-\alpha K_n^2t}\cos\frac{n\pi x}{L},\qquad
K_n=\frac{n\pi}{L},\quad n=1,2,\ldots.
$$

The [cosine](cosine.md) has zero [temperature gradient](temperature-gradient.md) at both ends, satisfying the insulated [Neumann boundary conditions](neumann-boundary-condition.md). Its spatial mean is zero, so [conservation of energy](conservation-of-energy.md) leaves the mean [temperature](temperature-split.md) $\overline T$ unchanged while the nonuniform part disappears. A short derivation substitutes $T=\overline T+A(t)\cos(K_nx)$ into the [heat equation](heat-equation.md): the second spatial [derivative](derivative.md) supplies $-K_n^2$, hence $A'=-\alpha K_n^2A$. The [exponential decay](exponential-decay.md) time is $\tau_n=1/(\alpha K_n^2)$; doubling angular [wavenumber](wavenumber.md) quarters this time. If cycles-per-[length](length.md) [spatial frequency](spatial-frequency.md) $f_x$ is used instead, $K=2\pi f_x$ and the rate is $4\pi^2\alpha f_x^2$.

<a id="image-insulated-bar-fourier-mode-decay-equal-thermal-conductivity-different-heat-capacities"></a>
![](thermal-diffusivity-insulated-fourier-mode-decay.png)

**[Figure 7](#image-insulated-bar-fourier-mode-decay-equal-thermal-conductivity-different-heat-capacities). Insulated-bar Fourier mode decay: equal thermal conductivity, different heat capacities**. Original constant-property model with $L=0.010\,\mathrm m$ and $n=1$. The normalized initial [temperature](temperature-split.md) profile is identical for both stipulated materials in [thermal diffusivity](thermal-diffusivity.md). The larger [volumetric heat capacity](volumetric-heat-capacity.md) gives a smaller [thermal diffusivity](thermal-diffusivity.md) and four times the decay time. Profiles at $t=10\,\mathrm s$ and amplitude histories are analytical predictions, not measured records.

For the two model materials in [thermal diffusivity](thermal-diffusivity.md) and $L=0.010\,\mathrm m$, $\tau_{1,A}\approx5.07\,\mathrm s$ and $\tau_{1,B}\approx20.3\,\mathrm s$. After $10\,\mathrm s$, the remaining amplitude fractions are approximately $0.139$ and $0.610$. A narrow hot-and-cold pattern disappears faster than a broad one because its [temperature](temperature-split.md) curvature, and hence the imbalance in conductive [heat flux](heat-flux-density.md), is larger.

## ↑ Ancestors (9)

1. [Thermal diffusion time](thermal-diffusion-time.md)
2. [Thermal diffusivity](thermal-diffusivity.md)
3. [Thermal conduction](thermal-conduction.md)
4. [Heat](heat-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Convective overstability growth rate](convective-overstability-growth-rate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-321/3/c/solution.md)
- [Thermal diffusion length](thermal-diffusion-length.md)
