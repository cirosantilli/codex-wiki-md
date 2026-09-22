# Two-level saturation population model

↑ **Parent:** [Doppler-free saturation spectroscopy](doppler-free-saturation-spectroscopy.md)

Choose a closed [two-level system](two-level-system.md), equal stimulated absorption and emission strengths, a monochromatic pump, and no extra [dephasing](dephasing-channel.md). Let $p_g+p_e=1$ be the lower and upper populations, and let [spontaneous emission](spontaneous-emission.md) remove upper population at rate $\Gamma=1/\tau_e$. In this convention the [natural linewidth](natural-linewidth.md) is [full width at half maximum](full-width-at-half-maximum.md) $\Gamma$ in [angular frequency](angular-frequency.md), its half width at half maximum is $\Gamma/2$, and its [full width at half maximum](full-width-at-half-maximum.md) in [hertz](hertz.md) is $\Gamma/(2\pi)$. All $\Delta$ below are angular detunings.

Let $s=I/I_{\rm sat}$ be the on-resonance [saturation parameter](saturation-parameter.md). An effective stimulated transition rate that reproduces the monochromatic steady response is

$$
R(\Delta)=\frac{\Gamma s}{2(1+4\Delta^2/\Gamma^2)},\qquad
\dot p_e=Rp_g-(R+\Gamma)p_e=R(1-2p_e)-\Gamma p_e.
$$

Here $R$ describes each stimulated direction, while $\Gamma$ describes irreversible [spontaneous emission](spontaneous-emission.md). The rate equation gives the steady populations; it is not a description of transient [Rabi oscillations](rabi-cycle.md). Setting $\dot p_e=0$ gives

$$
p_e=\frac{R}{\Gamma+2R}
=\frac{s}{2(1+s+4\Delta^2/\Gamma^2)},\qquad p_g=1-p_e,
$$

and the population difference relevant to net weak-probe [photon absorption](photon-absorption.md) is

$$
d=p_g-p_e=\frac{1+4\Delta^2/\Gamma^2}{1+s+4\Delta^2/\Gamma^2},\qquad
q=1-d=\frac{s}{1+s+4\Delta^2/\Gamma^2}.
$$

The pump depletes the lower population by $p_e$, but reduces the population difference by $q=2p_e$: [stimulated emission](stimulated-emission.md) contributes as well as missing ground-state absorbers. On resonance, $s=1$ gives $p_e=1/4$, $p_g=3/4$, $d=1/2$; $s=9$ gives $p_e=0.45$, $p_g=0.55$, $d=0.10$. As $s\to\infty$, the two populations approach $1/2$, rather than producing a [population inversion](population-inversion.md). Far off resonance, $p_e\to0$ and $d\to1$.

For moving atoms use $\Delta=\delta-kv$ in these pump-prepared populations. A weak counterpropagating probe interrogates them near $\delta+kv=0$. A simple population-only approximation to its [absorption coefficient](absorption-coefficient.md) averages the weak-probe [Lorentzian line shape](lorentzian-line-shape.md) times $d(\delta-kv)$ over the [Maxwell-Boltzmann velocity distribution](maxwell-boltzmann-velocity-distribution.md). It neglects interference between the beams, changes of [velocity](velocity.md) during illumination, and multilevel [optical pumping](optical-pumping.md). Those restrictions matter for real alkali [chemical atoms](atom-physics.md).

**Table of contents**

- [Power broadening](power-broadening.md)

## ↑ Ancestors (6)

1. [Doppler-free saturation spectroscopy](doppler-free-saturation-spectroscopy.md)
2. [Laser spectroscopy](laser-spectroscopy.md)
3. [Atomic measurement methods](atomic-measurement-methods.md)
4. [Atomic physics](atomic-physics-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Power broadening](power-broadening.md)
- [Sodium saturation spectroscopy experiment of 1971](sodium-saturation-spectroscopy-experiment-of-1971.md)
