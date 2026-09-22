<h1 id="resistive-damping-of-an-alfven-wave">Resistive damping of an Alfvén wave</h1>

↑ **Parent:** [Alfvén wave](alfven-wave.md)

Finite [electrical conductivity](electrical-conductivity.md) $\sigma$ allows [magnetic diffusion](magnetic-diffusion.md), with [magnetic diffusivity](magnetic-diffusivity.md) $\eta_m=1/(\mu_0\sigma)$. In the same uniform, unbounded geometry as the [Linear Alfvén wave equations](linear-alfven-wave-equations.md), neglect [viscosity](dynamic-viscosity-split.md) but add $\eta_m\partial_z^2\mathbf b_\perp$ to induction. For real $k_\parallel$ and time dependence $e^{-i\omega t}$, elimination gives

$$
\omega^2+i\eta_m k_\parallel^2\omega-v_A^2k_\parallel^2=0,
\qquad
\omega=-\frac{i\eta_m k_\parallel^2}{2}\pm\sqrt{v_A^2k_\parallel^2-\frac{\eta_m^2k_\parallel^4}{4}}.
$$

Thus weak [magnetic diffusion](magnetic-diffusion.md), $\eta_m|k_\parallel|\ll v_A$, gives an [amplitude](wave-amplitude.md) decay rate $\eta_m k_\parallel^2/2$. For $\eta_m|k_\parallel|>2v_A$, both temporal roots are purely decaying; they no longer describe an oscillating traveling mode. This temporal calculation at fixed real [wavenumber](wavenumber.md) is different from a driven vessel at fixed real [frequency](frequency.md), where a complex spatial [wavenumber](wavenumber.md) describes penetration and attenuation. [Viscosity](dynamic-viscosity-split.md) also dissipates [kinetic energy](kinetic-energy.md), and walls introduce transverse gradients and additional losses.

For an axial length $L$, comparing the [magnetic diffusion](magnetic-diffusion.md) time $L^2/\eta_m$ with the transit time $L/v_A$ gives the ratio $Lv_A/\eta_m$. A large value favors propagation before diffusion, but a narrow vessel can introduce a shorter transverse diffusion scale. In the actual 1949 analysis, finite [electrical conductivity](electrical-conductivity.md) and vessel dimensions restrict the useful [frequency](frequency.md) interval; above its upper limit the response becomes a skin wave.[Abstract: finite-conductivity frequency interval, upper limit and geometrical lower limit](experimental-investigations-of-magneto-hydrodynamic-waves-by-stig-lundquist.md)

## ↑ Ancestors (9)

1. [Alfvén wave](alfven-wave.md)
2. [Magnetohydrodynamic wave](magnetohydrodynamic-wave.md)
3. [Ideal magnetohydrodynamics](ideal-magnetohydrodynamics-split.md)
4. [Magnetohydrodynamics](magnetohydrodynamics-split.md)
5. [Astrophysical fluid dynamics](astrophysical-fluid-dynamics-split.md)
6. [Fluid mechanics](fluid-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
