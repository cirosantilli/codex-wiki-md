# Passive membrane response in current clamp

↑ **Parent:** [Current clamp](current-clamp.md)

Model a spatially uniform [cell membrane](cell-membrane.md) as a [capacitor](capacitor.md) of [membrane capacitance](membrane-capacitance.md) $C_m$ in parallel with membrane [electrical resistance](electrical-resistance.md) $R_m$ and a fixed leak [reversal potential](reversal-potential.md) $E_L$. Exclude active [ion channels](ion-channel.md), [seal leak current](seal-leak-current.md) and pipette [capacitance](capacitance.md). For [electric current](electric-current.md) $I$ injected into the [biological cell](biological-cell.md), [electric charge conservation](charge-conservation.md) yields

$$
C_m\frac{dV}{dt}=I-\frac{V-E_L}{R_m}.
$$

Starting at $V(0)=E_L$ and applying constant $I$ gives the [ordinary differential equation](ordinary-differential-equation.md) solution

$$
V(t)=E_L+IR_m\left(1-e^{-t/\tau_m}\right),\qquad \tau_m=R_mC_m.
$$

The [steady state](steady-state.md) rise is $IR_m$; the [time constant](time-constant.md) is $R_mC_m$. With $I=50\,\mathrm{pA}$, $R_m=200\,\mathrm{M\Omega}$, $C_m=50\,\mathrm{pF}$ and $E_L=-70\,\mathrm{mV}$, the rise is $10\,\mathrm{mV}$ and $\tau_m=10\,\mathrm{ms}$. At one [time constant](time-constant.md) the rise is $10(1-e^{-1})\,\mathrm{mV}\approx6.321\,\mathrm{mV}$. The figure's uncompensated pipette voltage adds $IR_s=1\,\mathrm{mV}$ for $R_s=20\,\mathrm{M\Omega}$. The membrane voltage is continuous at step onset in this model, while the pipette voltage immediately acquires that access drop.

Checking the units is instructive: [electrical resistance](electrical-resistance.md) times [capacitance](capacitance.md) has units $\Omega\,\mathrm F=\mathrm s$, and [electric current](electric-current.md) times [electrical resistance](electrical-resistance.md) has units of voltage. Unlike the passive [voltage clamp](voltage-clamp.md) transient under [patch-clamp series resistance](patch-clamp-series-resistance.md), this ideal [current clamp](current-clamp.md) membrane [time constant](time-constant.md) is set by $R_mC_m$, not $R_sC_m$. Strong current steps can recruit [voltage-gated ion channels](voltage-gated-ion-channel.md); the passive model then fails and cannot generate an [action potential](action-potential.md). Small pulses of both signs, stable access and repeated baseline measurements help test whether the passive approximation is appropriate.

## ↑ Ancestors (5)

1. [Current clamp](current-clamp.md)
2. [Patch clamp](patch-clamp.md)
3. [Neuroscience](neuroscience.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)
