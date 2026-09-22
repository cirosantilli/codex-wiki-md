# Electrical impedance

↑ **Parent:** [Electrical circuit](electrical-circuit-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electrical_impedance)

[Electrical impedance](electrical-impedance.md) is the ratio of terminal [electric potential difference](electric-potential-difference.md) and [electric current](electric-current.md) [phasors](phasor.md) at one specified positive [angular frequency](angular-frequency.md) $\omega$. For an [electrical circuit](electrical-circuit-split.md) modeled as a [linear time-invariant system](linear-time-invariant-system.md), use the sinusoidal [steady state](steady-state.md) after any decaying transient has settled. With the [passive sign convention](passive-sign-convention.md), positive [electric current](electric-current.md) enters the terminal assigned positive [electric potential difference](electric-potential-difference.md). Define peak [complex amplitudes](complex-amplitude.md) by

$$
v(t)=\operatorname{Re}(\widehat V e^{\mathrm i\omega t}),\qquad
i(t)=\operatorname{Re}(\widehat I e^{\mathrm i\omega t}),\qquad
Z(\omega)=\frac{\widehat V}{\widehat I},\quad \widehat I\ne0.
$$

The physical $v(t)$ and $i(t)$ are real; the [complex numbers](complex-number.md) encode their [amplitudes](wave-amplitude.md) and [wave phases](phase-waves.md). The unit of [electrical impedance](electrical-impedance.md) is the [ohm](ohm.md), $1\,\Omega=1\,\mathrm V/\mathrm A$. Both [phasors](phasor.md) may instead use [root mean square](root-mean-square.md) magnitudes, with the same ratio $Z$. A nonlinear [diode](diode.md) can generate additional [frequencies](frequency.md); a single $Z(\omega)$ then does not describe the whole response.

Write the [electrical impedance](electrical-impedance.md) in Cartesian and [polar forms](polar-form-of-a-complex-number.md) as

$$
Z=R+\mathrm iX=|Z|e^{\mathrm i\phi},\qquad
R=\operatorname{Re}Z,\quad X=\operatorname{Im}Z,\quad
|Z|=\sqrt{R^2+X^2},\quad
\phi=\arg Z=\arg\widehat V-\arg\widehat I.
$$

Here $R$ is the resistive [real part](real-part.md), $X$ the signed [electrical reactance](electrical-reactance.md), and $\phi$ the voltage-minus-current [phase difference](phase-difference.md), defined modulo a full turn. The [Pythagorean theorem](pythagorean-theorem.md) gives the [modulus](modulus.md) from a [right triangle](right-triangle.md) in the [complex plane](complex-plane.md). The [complex argument](argument-complex-analysis.md) gives the rotation from the current [phasor](phasor.md) to the voltage [phasor](phasor.md). Thus $V_{\rm rms}=|Z|I_{\rm rms}$, while negative $\phi$ means [electric current](electric-current.md) leads terminal [electric potential difference](electric-potential-difference.md). For $R>0$, $\phi=\arctan(X/R)$ lies between $-\pi/2$ and $\pi/2$; outside that case, use the quadrant of the [complex number](complex-number.md) rather than a bare [inverse tangent](inverse-tangent.md). The geometric magnitude and [phase difference](phase-difference.md) are the two pieces of the AC relation.[§15.3, figures 15.12–15.13 and equations 15.9–15.11: phasor addition, phase angle, impedance magnitude and ohm unit](university-physics-volume-2-by-samuel-j-ling-and-others.md)

<a id="image-electrical-impedance-as-a-complex-number-and-a-voltage-current-phase-difference"></a>
![](impedance-phasor-components-and-timing.png)

**[Figure 7](#image-electrical-impedance-as-a-complex-number-and-a-voltage-current-phase-difference). Electrical impedance as a complex number and a voltage-current phase difference**. Original ideal [series RC impedance](series-rc-impedance.md) calculation: $R=100\,\Omega$, $C=1\,\mu\mathrm F$, $f=1000\,\mathrm{Hz}$. Left: $Z=100-159.155\mathrm i\,\Omega$, resolved into its [real part](real-part.md) and signed [electrical reactance](electrical-reactance.md). Right: normalized predicted [sinusoids](sinusoid.md) with the current [phasor](phasor.md) as the zero-phase reference; their peak separation is $0.160717\,\mathrm{ms}$. The plotted normalized heights do not compare volts with amperes.

Multiplication by $Z$ acts on [phasors](phasor.md), not on instantaneous physical signals. For example, when $i(t)=I_0\cos\omega t$,

$$
v(t)=I_0\bigl(R\cos\omega t-X\sin\omega t\bigr).
$$

The second term is in [phase quadrature](phase-quadrature.md) with [electric current](electric-current.md); it cannot be represented by pointwise multiplication $v(t)=Zi(t)$ when $X\ne0$. This is the useful compression: one [complex multiplication](complex-multiplication.md) replaces separate [amplitude](wave-amplitude.md) and [phase difference](phase-difference.md) calculations, while the [real part](real-part.md) restores the physical signal.

An ideal [resistor](resistor.md), [inductor](inductor.md) and [capacitor](capacitor.md) have $Z_R=R$, $Z_L=\mathrm i\omega L$ and $Z_C=1/(\mathrm i\omega C)$. Their [electrical impedances](electrical-impedance.md) add in a [series RLC circuit](series-rlc-circuit.md), giving $Z=R+\mathrm i(\omega L-1/(\omega C))$. The current [amplitude](wave-amplitude.md) is $V_0/|Z|$, so cancellation of the [imaginary parts](imaginary-part.md) explains the [resonant series RLC response](resonant-series-rlc-response.md). The component-law derivation and opposite [complex exponential](complex-exponential-function.md) convention are in [reactance phase convention](reactance-phase-convention.md).

**Table of contents**

- [Input impedance](input-impedance.md)
- [Impedance matching](impedance-matching.md)
  - [Matched load](matched-load.md)
  - [Maximum power transfer theorem](maximum-power-transfer-theorem.md)
  - [Quarter-wave impedance transformer](quarter-wave-impedance-transformer.md)
- [Lossy parallel coil resonance](lossy-parallel-coil-resonance.md)
  - [Determining a lossy parallel coil from its admittance](determining-a-lossy-parallel-coil-from-its-admittance.md)
- [Electrical admittance](electrical-admittance.md)
  - [Electrical susceptance](electrical-susceptance.md)
- [Series RC impedance](series-rc-impedance.md)
- [Electrical impedance phase measurement](electrical-impedance-phase-measurement.md)
- [Electrical reactance](electrical-reactance.md)
  - [Reactance phase convention](reactance-phase-convention.md)
  - [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md)
- [Output impedance](output-impedance.md)

## ↑ Ancestors (5)

1. [Electrical circuit](electrical-circuit-split.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (32)

- [Capacitance measurement calibration](capacitance-measurement-calibration.md)
- [Dielectric capacitance measurement](dielectric-capacitance-measurement.md)
- [Electrical admittance](electrical-admittance.md)
- [Electrical impedance](electrical-impedance.md)
- [Electrical impedance phase measurement](electrical-impedance-phase-measurement.md)
- [Electrical noise reduction](electrical-noise-reduction.md)
- [Electrical reactance](electrical-reactance.md)
- [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md)
- [Impedance matching](impedance-matching.md)
- [Inverting low-pass amplifier](inverting-low-pass-amplifier.md)
- [Lossy parallel coil resonance](lossy-parallel-coil-resonance.md)
- [Open circuit](open-circuit.md)
- [Output impedance](output-impedance.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021/section-a/a2/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-a/5/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-a/a5/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-b/b6/e/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2/section-b/b6/c/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/section-c/c11/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-c/11/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/section-a/2/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/section-b/8/a/solution.md)
- [RC low-pass frequency response](rc-low-pass-frequency-response.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [RL low-pass filter](rl-low-pass-filter.md)
- [Series RC impedance](series-rc-impedance.md)
- [Short circuit](short-circuit.md)
- [Shot noise photocurrent measurement](shot-noise-photocurrent-measurement.md)
- [Thermal noise measurement](thermal-noise-measurement.md)
- [Wien bridge](wien-bridge.md)
