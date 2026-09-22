# Atomic clock frequency shifts

↑ **Parent:** [Atomic clock](atomic-clock.md)

A narrow fringe makes the center easier to resolve statistically; it does not certify an unbiased [frequency](frequency.md). For example, with ideal $\pi/2$ pulses and a second-pulse [oscillation phase](phase-waves.md) offset $\varphi_c$, the [finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md) approaches

$$
P_{g\to e}=\cos^2\!\left(\frac{\delta T-\varphi_c}{2}\right),\qquad
\nu_{\mathrm{center}}-\nu_0=-\frac{\varphi_c}{2\pi T}.
$$

This sign uses exactly the [Rabi detuning](rabi-detuning.md) convention and pulse [Hamiltonian operator](hamiltonian-quantum-mechanics.md) above, with the second pulse replacing $\sigma_x$ by $\cos\varphi_c\,\sigma_x+\sin\varphi_c\,\sigma_y$. The factor $2\pi$ converts [angular frequency](angular-frequency.md) to ordinary [frequency](frequency.md). For the original example, $\varphi_c=0.010$ rad and $T=5\,\mathrm{ms}$ give a shift of about $-0.318\,\mathrm{Hz}$. For finite pulses or distributed flight times, use the full signal and its [atomic clock frequency lock](atomic-clock-frequency-lock.md) rather than inserting an unweighted mean $T$.

NIST-7 used [optical pumping](optical-pumping.md) and [fluorescence](fluorescence-split.md). Controls included field-sensitive transitions, independent beam-speed measurements, [microwave](microwave.md) power stabilization, and beam reversal for cavity [quantum phase](quantum-phase.md) errors.[§2.2, pp. 50–52: optical readout and frequency-shift controls](primary-atomic-frequency-standards-at-nist-by-d-b-sullivan-and-others.md)

The connection to [special relativity](special-relativity-split.md) is quantitative. A freely moving emitter's [proper time](proper-time.md) advances more slowly than laboratory time by $\sqrt{1-v^2/c^2}$. With first-order propagation effects removed in the ideal comparison, its internal laboratory [frequency](frequency.md) is therefore

$$
\frac{\nu_{\mathrm{lab}}-\nu_0}{\nu_0}\simeq-\frac{v^2}{2c^2}.
$$

Correcting an ensemble signal requires the effective [velocity](velocity.md) weights of preparation, interrogation and detection, not simply the oven's mean [speed](speed.md). Additional shifts from [Zeeman splitting](zeeman-splitting.md), unwanted light, [collisions](collision.md) and cavity fields likewise require separate evaluation; [feedback control](closed-loop-control.md) locks to the observed line, including any uncorrected bias. Comparing clocks at different [gravitational potentials](newtonian-potential-of-a-point-mass.md) additionally requires [gravitational time dilation](gravitational-time-dilation.md). The moving-clock experiments in [twin paradox clock experiments](twin-paradox-clock-experiments.md) compare calibrated clock readings along different [world lines](world-line.md); the beam atoms' internal motion is part of the clock mechanism's own correction.

## ↑ Ancestors (9)

1. [Atomic clock](atomic-clock.md)
2. [Twin paradox clock experiments](twin-paradox-clock-experiments.md)
3. [Twin paradox](twin-paradox.md)
4. [Time dilation](time-dilation.md)
5. [Lorentz factor](lorentz-factor.md)
6. [Special relativity](special-relativity-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Ramsey frequency precision](ramsey-frequency-precision.md)
- [Velocity-averaged Ramsey line](velocity-averaged-ramsey-line.md)
