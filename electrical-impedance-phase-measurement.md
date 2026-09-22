# Electrical impedance phase measurement

↑ **Parent:** [Electrical impedance](electrical-impedance.md)

An actual teaching experiment turns the [phasor](phasor.md) definition into readings. Leipzig University's laboratory handout Measurements with an oscilloscope, experiment E 3e, uses a [function generator](function-generator.md), a two-channel [oscilloscope](oscilloscope.md), a known [resistor](resistor.md) and a [capacitor](capacitor.md). Figure 5 places the [capacitor](capacitor.md) above the [resistor](resistor.md), with a common return below the [resistor](resistor.md). Channel 1 measures the applied terminal [electric potential difference](electric-potential-difference.md) $v_1$; channel 2 measures $v_R$. The handout asks for peak-to-peak values and relative timing, then comparison of measured and calculated [electrical impedances](electrical-impedance.md) with $R=3\,\mathrm{k\Omega}$, $C=0.47\,\mu\mathrm F$ at $100$ and $300\,\mathrm{Hz}$. It also asks students to check the oscilloscope time base against a digitally counted generator [frequency](frequency.md). These are apparatus and procedural specifications, not reported measured results.[Measurements with an oscilloscope, E 3e, p. 1 tasks 1 and 4; pp. 5–6 Measurement of impedances, figure 5 and experimental comparison](measurements-with-an-oscilloscope-experiment-e-3e-physikalisches-grundpraktikum-universitat-leipzig.md)

For this arrangement, [Ohm's law](ohm-s-law.md) gives $i(t)=v_R(t)/R$ if probe loading and the sensing [resistor](resistor.md)'s [electrical reactance](electrical-reactance.md) are negligible. Record both voltage magnitudes with the same convention: peak, peak-to-peak, or [root mean square](root-mean-square.md). After the transient settles, compare matched rising zero crossings $t_1$ of $v_1$ and $t_R$ of $v_R$, with [period](period-of-a-function.md) $T=1/f$. Then

$$
|Z|=R\frac{V_1}{V_R},\qquad
\Delta t=t_R-t_1,\qquad
\phi=\frac{2\pi\Delta t}{T},\qquad
Z=|Z|(\cos\phi+\mathrm i\sin\phi).
$$

The recovered [electrical impedance](electrical-impedance.md) includes the known [resistor](resistor.md). For a separate unknown component in series with that [resistor](resistor.md), subtract $R$ from the inferred total [electrical impedance](electrical-impedance.md). A current crossing earlier than the applied voltage crossing gives $\Delta t<0$, hence negative $\phi$. For the stipulated [series RC impedance](series-rc-impedance.md) example at $1000\,\mathrm{Hz}$, this predicts $\Delta t=-0.160717\,\mathrm{ms}$; it is a calculated timing, not a lab observation. Timing supplies the [complex argument](argument-complex-analysis.md) that an amplitude ratio alone cannot recover.

As additional measurement controls, first feed the same [sinusoid](sinusoid.md) to both channels to check relative delay and polarity; then replace the reactive chain with a known [resistor](resistor.md), expecting nearly zero [phase difference](phase-difference.md). Keep both probe returns at the common return shown in figure 5. A reversed voltage polarity adds half a turn to its inferred [wave phase](phase-waves.md). Match crossings with the same slope and choose $-T/2<\Delta t\leq T/2$; adjacent cycles otherwise change $\phi$ by a full turn. A sweep continuous in [frequency](frequency.md) helps track that branch. These controls test the signed inference rather than assuming that the scope's delay readout has the desired sign.

Measure the loaded terminal [electric potential difference](electric-potential-difference.md) on channel 1 at every [frequency](frequency.md). The generator's [output impedance](output-impedance.md) can change the applied magnitude; its front-panel setting is not the measured terminal value. The generator's internal [electrical impedance](electrical-impedance.md) is outside the terminal ratio above, while the known sensing [resistor](resistor.md) is inside it. Probe loading, finite timing resolution, component tolerances and distorted waveforms limit the inference. A repeat at lower drive [amplitude](wave-amplitude.md) tests whether one linear [electrical impedance](electrical-impedance.md) still fits. [Electrical reactance bench measurement](electrical-reactance-bench-measurement.md) develops these loading and reference-direction issues further.

## ↑ Ancestors (6)

1. [Electrical impedance](electrical-impedance.md)
2. [Electrical circuit](electrical-circuit-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
