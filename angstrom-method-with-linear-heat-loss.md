<h1 id="angstrom-method-with-linear-heat-loss">Ångström method with linear heat loss</h1>

↑ **Parent:** [Ångström periodic heating method](angstrom-periodic-heating-method.md)

Side losses need not destroy the method. Let $\theta$ be the small [temperature](temperature-split.md) disturbance about a steady background in surroundings at fixed [temperature](temperature-split.md). For a rod of cross-sectional [area](surface-area.md) $S$ and perimeter $\mathcal P$, a uniform real surface [heat transfer coefficient](heat-transfer-coefficient.md) $h_s$ produces a loss per unit [volume](volume.md) of $H\theta$, with $H=h_s\mathcal P/S$. Assume constant $k,\rho,c_p,H$, a cross-section nearly uniform in [temperature](temperature-split.md), and no distributed heat source. The balance becomes

$$
\rho c_p\partial_t\theta=k\partial_x^2\theta-H\theta,\qquad
\partial_t\theta=\alpha\partial_x^2\theta-\lambda\theta,\qquad
\lambda=\frac{H}{\rho c_p}\geq0.
$$

Here $H$ has units $\mathrm{W\,m^{-3}\,K^{-1}}$, while $\lambda$ has units $\mathrm{s^{-1}}$. This is a distributed version of [Newton's law of cooling](newton-s-law-of-cooling.md); a constant linearized contribution from [thermal radiation](thermal-radiation.md) may be included over a small [temperature](temperature-split.md) range. It does not represent arbitrary time-dependent coupling to a surrounding material with its own thermal storage.

For the decaying exponential branch, the [phasor](phasor.md) equation gives

$$
\gamma^2=\frac{\lambda+i\omega}{\alpha},\qquad
a^2-b^2=\frac{\lambda}{\alpha},\qquad
2ab=\frac{\omega}{\alpha},
$$

so that

$$
a=\sqrt{\frac{\sqrt{\lambda^2+\omega^2}+\lambda}{2\alpha}},\qquad
b=\sqrt{\frac{\sqrt{\lambda^2+\omega^2}-\lambda}{2\alpha}}.
$$

Real positive side loss increases $a$ and decreases $b$ at fixed [angular frequency](angular-frequency.md) and [thermal diffusivity](thermal-diffusivity.md). Their product eliminates $\lambda$, yielding the combined inference

$$
\boxed{\alpha=\frac{\omega}{2ab}
=\frac{\omega\Delta x^2}{2\log(A_1/A_2)\,\Delta\phi}
=\frac{\Delta x^2}{2\log(A_1/A_2)\,\Delta t}},\qquad
\Delta t=\frac{\Delta\phi}{\omega}.
$$

This result requires that attenuation and lag belong to the same exponential [complex wavenumber](complex-wavenumber.md) at the same [frequency](frequency.md), and that the loss term is real. It does not generally survive a superposition caused by a nearby finite end, spatially varying coefficients, transverse [temperature gradients](temperature-gradient.md), or unequal sensor delays. The inferred $\lambda=\alpha(a^2-b^2)$ supplies an additional model check; a negative value signals inconsistency with this passive-loss model rather than negative physical cooling.

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
