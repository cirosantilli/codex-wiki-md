# Thermal diffusion wave

↑ **Parent:** [Ångström periodic heating method](angstrom-periodic-heating-method.md)

A [thermal diffusion wave](thermal-diffusion-wave.md) is a periodically forced solution of the [heat equation](heat-equation.md), with spatially decreasing [amplitude](wave-amplitude.md) and varying [wave phase](phase-waves.md). In a semi-infinite rod $x\geq0$, assume constant [thermal diffusivity](thermal-diffusivity.md), negligible side losses, a nearly uniform [temperature](temperature-split.md) across each cross-section, and the [boundary conditions](boundary-condition.md) $\theta(0,t)=\Theta_0\cos\omega t$ and $\theta(x,t)\to0$ as $x\to\infty$. A [steady periodic thermal state](steady-periodic-thermal-state.md) then satisfies

$$
\partial_t\theta=\alpha\partial_x^2\theta,\qquad
\widehat\theta(x)=\Theta_0e^{-\gamma x},\qquad
\gamma^2=\frac{i\omega}{\alpha},\qquad
\gamma=a+ib=(1+i)\sqrt{\frac{\omega}{2\alpha}}.
$$

Choose the [square root](square-root.md) in the [complex numbers](complex-number.md) with $a>0$ so that the [amplitude](wave-amplitude.md) decays into the rod. Substitution of the [phasor](phasor.md) into the [heat equation](heat-equation.md) proves the formula: $i\omega\widehat\theta=\alpha\widehat\theta''$. Taking the real part gives the displayed [cosine](cosine.md). In this convention $a$ is the spatial attenuation slope and $b$ is the spatial lag slope, both in $\mathrm{m^{-1}}$; $\gamma$ combines them into one [complex number](complex-number.md). If a [complex wavenumber](complex-wavenumber.md) $K$ is defined by $e^{i\omega t-iKx}$ instead, $K=b-ia$.

With $\Delta x=x_2-x_1>0$, let $A_j=|\widehat\theta(x_j)|$ and define a positive downstream lag $\Delta\phi$. Then

$$
D=\log\frac{A_1}{A_2}=a\Delta x,\qquad
\Delta\phi=b\Delta x,\qquad
a=b\quad\text{without side losses},
$$

and either measurement determines [thermal diffusivity](thermal-diffusivity.md):

$$
\alpha=\frac{\omega\Delta x^2}{2D^2}
=\frac{\omega\Delta x^2}{2(\Delta\phi)^2}.
$$

The [logarithm](logarithm.md) uses an [amplitude](wave-amplitude.md) ratio, not a ratio of squared [amplitudes](wave-amplitude.md). The lag is in [radians](radian.md) and must be tracked continuously across cycles: a measured [phase difference](phase-difference.md) modulo $2\pi$ leaves an integer-cycle ambiguity. Use closer sensor spacings or vary [frequency](frequency.md) continuously to resolve that ambiguity. Equal attenuation and lag slopes provide a useful diagnostic of the no-side-loss model.

The apparent [phase velocity](phase-velocity.md) is $\omega/b=\sqrt{2\alpha\omega}$, which depends on [frequency](frequency.md). A [thermal diffusion wave](thermal-diffusion-wave.md) therefore does not give a material-independent travel speed for [heat](heat-split.md); it is a forced pattern in a dissipative [diffusion equation](diffusion-equation-split.md). The ideal [heat equation](heat-equation.md) still has [infinite propagation speed](infinite-propagation-speed.md), and the observed lag is not the arrival time of a sharp front.

**Table of contents**

- [Thermal penetration depth](thermal-penetration-depth.md)

## ↑ Ancestors (9)

1. [Ångström periodic heating method](angstrom-periodic-heating-method.md)
2. [Thermal diffusivity](thermal-diffusivity.md)
3. [Thermal conduction](thermal-conduction.md)
4. [Heat](heat-split.md)
5. [Thermodynamics](thermodynamics-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Complex wavenumber](complex-wavenumber.md)
- [Thermal diffusion wave](thermal-diffusion-wave.md)
- [Thermal penetration depth](thermal-penetration-depth.md)
