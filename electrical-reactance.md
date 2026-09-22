# Electrical reactance

↑ **Parent:** [Electrical impedance](electrical-impedance.md)

Electrical reactance $X$ is the signed [imaginary part](imaginary-part.md) of [electrical impedance](electrical-impedance.md) $Z=R+\mathrm iX$, measured in [ohms](ohm.md). It describes the part of the terminal [electric potential difference](electric-potential-difference.md) in [phase quadrature](phase-quadrature.md) with the [electric current](electric-current.md) in a sinusoidal [steady state](steady-state.md). In the $e^{\mathrm i\omega t}$ convention, an ideal [inductor](inductor.md) has $X_L=\omega L>0$ and an ideal [capacitor](capacitor.md) has $X_C=-1/(\omega C)<0$ for $\omega>0$. A large $|X|$ reduces [electric current](electric-current.md) at fixed applied voltage, but an ideal purely reactive component returns the [energy](energy-split.md) it receives over each cycle. This is why [electrical reactance](electrical-reactance.md) and [electrical resistance](electrical-resistance.md) have the same units yet describe different physical behavior. [Feynman, Leighton and Sands, The Feynman Lectures on Physics, II.22.5: resistance, reactance and energy loss](https://www.feynmanlectures.caltech.edu/II_22.html#Ch22-S5).

<a id="image-signed-electrical-reactances-cancel-in-a-toy-series-rlc-circuit"></a>
![](reactance-frequency-cancellation.png)

**[Figure 9](#image-signed-electrical-reactances-cancel-in-a-toy-series-rlc-circuit). Signed electrical reactances cancel in a toy series RLC circuit**. Calculated ideal curves, not measured data: [inductance](inductance.md) $L=10\,\mathrm{mH}$, [capacitance](capacitance.md) $C=1\,\mu\mathrm F$, total [electrical resistance](electrical-resistance.md) $R_\Sigma=100+10=110\,\Omega$, and applied [root mean square](root-mean-square.md) voltage $1.00\,\mathrm V$. The $10\,\Omega$ is the sensing [resistor](resistor.md) in [electrical reactance bench measurement](electrical-reactance-bench-measurement.md). Top: $X_L$, signed $X_C$, and their sum. Bottom: [electric current](electric-current.md) and voltage-minus-current [phase difference](phase-difference.md). At $f_0=1.592\,\mathrm{kHz}$ the sum vanishes, the [electric current](electric-current.md) peaks, and terminal voltage and [electric current](electric-current.md) are in phase.

In a [series RLC circuit](series-rlc-circuit.md), [electrical impedances](electrical-impedance.md) add because the same [electric current](electric-current.md) passes through every component. For ideal positive [inductance](inductance.md) $L$, [capacitance](capacitance.md) $C$, and total [electrical resistance](electrical-resistance.md) $R_\Sigma>0$,

$$
X(\omega)=\omega L-\frac1{\omega C},\qquad
|Z|=\sqrt{R_\Sigma^2+X^2},\qquad
I_{\rm rms}=\frac{V_{\rm rms}}{|Z|},\qquad
\phi=\arctan\frac{X}{R_\Sigma}.
$$

Here $\phi$ is voltage [wave phase](phase-waves.md) minus current [wave phase](phase-waves.md). Below $\omega_0=1/\sqrt{LC}$, $X<0$ and [electric current](electric-current.md) leads terminal voltage; above it, $X>0$ and [electric current](electric-current.md) lags. At $\omega_0$, the two signed [electrical reactances](electrical-reactance.md) cancel, leaving $Z=R_\Sigma$ and the maximum [electric current](electric-current.md) at fixed terminal voltage. This is the [resonant series RLC response](resonant-series-rlc-response.md). [Electrical resistance](electrical-resistance.md) does not cancel: the toy circuit gives $f_0=\omega_0/(2\pi)=1591.55\,\mathrm{Hz}$ and $I_{\rm rms}=9.091\,\mathrm{mA}$ there. These numbers follow directly from the stipulated component values. [Ling, Moebs and Sanny, University Physics 2, §15.3: series impedance and resonance](university-physics-volume-2-by-samuel-j-ling-and-others.md).

Cancellation concerns terminal voltage, not the disappearance of stored [energy](energy-split.md). In the toy circuit at [resonance](resonance.md), the individual [inductor](inductor.md) and [capacitor](capacitor.md) voltages are each $0.9091\,\mathrm V$ in [root mean square](root-mean-square.md) magnitude, with opposite [wave phases](phase-waves.md), while their sum is zero. Their peak stored [magnetic energy](magnetic-energy.md) and [capacitor energy](capacitor-energy.md) are each $0.8264\,\mu\mathrm J$, attained at different times. With smaller positive $R_\Sigma$, either component voltage can exceed the applied voltage. This ability to select a [frequency](frequency.md) while sustaining internal [energy](energy-split.md) exchange connects [electrical reactance](electrical-reactance.md) to tuning and [frequency response](frequency-response.md).

For an ideal [inductor](inductor.md) or [capacitor](capacitor.md), the absorbed instantaneous [power](power.md) equals the rate of change of stored [energy](energy-split.md):

$$
p_L=v_Li=\frac{d}{dt}\left(\frac12Li^2\right),\qquad
p_C=v_Ci=\frac{d}{dt}\left(\frac12Cv_C^2\right).
$$

Positive [power](power.md) stores [energy](energy-split.md); negative [power](power.md) returns it. Over a periodic [steady state](steady-state.md), each stored [energy](energy-split.md) returns to its initial value, so its cycle-averaged absorbed [power](power.md) is zero. An ideal [resistor](resistor.md) instead has $p_R=Ri^2\geq0$, transferring [energy](energy-split.md) into [Joule heating](joule-heating.md). More generally, the average terminal [power](power.md) of this [series RLC circuit](series-rlc-circuit.md) is

$$
\overline p=V_{\rm rms}I_{\rm rms}\cos\phi=I_{\rm rms}^2R_\Sigma.
$$

Zero average [power](power.md) in an ideal reactive component does not imply zero instantaneous [power](power.md), zero [electric current](electric-current.md), or zero stored [energy](energy-split.md). Real coils and [capacitors](capacitor.md) have losses, so zero ideal reactive loss is a model assumption rather than a claim about every component. [Ling, Moebs and Sanny, University Physics 2, §15.4: instantaneous and average AC power](university-physics-volume-2-by-samuel-j-ling-and-others.md).

**Table of contents**

- [Reactance phase convention](reactance-phase-convention.md)
- [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md)

## ↑ Ancestors (6)

1. [Electrical impedance](electrical-impedance.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Electrical impedance](electrical-impedance.md)
- [Electrical impedance phase measurement](electrical-impedance-phase-measurement.md)
- [Electrical reactance](electrical-reactance.md)
- [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md)
- [Resonant series RLC response](resonant-series-rlc-response.md)
- [Series RC impedance](series-rc-impedance.md)
