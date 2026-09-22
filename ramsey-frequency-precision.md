# Ramsey frequency precision

↑ **Parent:** [Ramsey spectroscopy](ramsey-spectroscopy.md)

The [full width at half maximum](full-width-at-half-maximum.md) of a fringe, the lifetime of [quantum coherence](quantum-coherence-in-a-specified-basis.md), and the precision of an estimated [frequency](frequency.md) are different quantities. In the ideal short-pulse limit, write the transfer [probability](probability.md) with contrast $0<V\leq1$ and second-pulse [oscillation phase](phase-waves.md) $\varphi$ as

$$
P=\frac{1+V\cos(\delta T-\varphi)}2,\qquad \delta=2\pi(\nu_0-\nu).
$$

At quadrature, $P=1/2$ and $|\partial P/\partial\nu|=\pi VT$. For $N$ independent, equally prepared particles with ideal binary readout, the [binomial distribution](binomial-distribution.md) gives $\sigma_P=\sqrt{P(1-P)/N}=1/(2\sqrt N)$. Local [propagation of uncertainty](propagation-of-uncertainty.md) therefore yields the displayed $\sigma_\nu$. For chosen $T=5\,\mathrm{ms}$, $V=0.8$ and $N=10^4$, it is approximately $0.398\,\mathrm{Hz}$, although the ideal fringe width is $100\,\mathrm{Hz}$. This is an original counting-noise estimate at a known quadrature, not the accuracy of a historical clock or a guarantee of finding the correct fringe.

For the illustrative [dephasing](dephasing-channel.md) model $V(T)=e^{-T/T_2}$ with fixed $N$, minimizing $\sigma_\nu$ maximizes $Te^{-T/T_2}$ and gives $T=T_2$: its [derivative](derivative.md) is $e^{-T/T_2}(1-T/T_2)$. This conclusion changes if longer interrogation reduces the number of accepted particles or the repetition rate. [Quantum decoherence](quantum-decoherence.md), a distribution of flight times, reference [oscillator](oscillator.md) noise and readout errors can reduce contrast; a fitted decay time need not identify one microscopic mechanism. More counting can improve precision while a reproducible cavity [quantum phase](quantum-phase.md) offset still biases the [frequency](frequency.md), as in [atomic clock frequency shifts](atomic-clock-frequency-shifts.md).

## ↑ Ancestors (15)

1. [Ramsey spectroscopy](ramsey-spectroscopy.md)
2. [Ramsey separated oscillatory fields experiment](ramsey-separated-oscillatory-fields-experiment.md)
3. [Ramsey interferometry](ramsey-interferometry.md)
4. [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md)
5. [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)
6. [Time-evolution operator](time-evolution-operator.md)
7. [Unitary time evolution](unitary-time-evolution.md)
8. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
9. [Observable](observable.md)
10. [Quantum state](quantum-state.md)
11. [Quantum system](quantum-system-split.md)
12. [Quantum mechanics](quantum-mechanics-split.md)
13. [Branches of physics](branches-of-physics.md)
14. [Physics](physics-split.md)
15. [Codex Wiki](split.md)
