# Finite-pulse Ramsey phase response

↑ **Parent:** [Finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md)

Keep the first pulse's [oscillation phase](phase-waves.md) zero and give the second phase $\varphi$ in the [Driven two-level Rabi model](driven-two-level-rabi-model.md). Its upper off-diagonal [Hamiltonian operator](hamiltonian-quantum-mechanics.md) entry is $\hbar\Omega e^{-i\varphi}/2$. Multiplying the two pulse [unitary operators](unitary-operator.md) and the free-flight [unitary operator](unitary-operator.md) gives

$$
\langle e|U_p(\varphi)U_fU_p(0)|g\rangle
=-2i e^{-i\varphi/2}\frac{\Omega}{q}s_p
\left[c_p\cos\frac{\delta T-\varphi}{2}-b\sin\frac{\delta T-\varphi}{2}\right].
$$

The [Born rule](born-rule.md) gives the displayed phase-dependent form using the $p,b,\theta$ of the [Ramsey fringe envelope](ramsey-fringe-envelope.md). Thus $\varphi=0$ reproduces the existing expression, while $\varphi=\pi$ turns a resonant transfer maximum into zero transfer. A single pulse's population is insensitive to its drive phase; the second coherent interaction makes their difference observable. An uncontrolled, uniformly random $\varphi$ instead averages this [probability](probability.md) to $2p(1-p)$, leaving the broad pulse response but removing the dark-flight fringes.

Finite pulses also contribute to the near-resonant [frequency](frequency.md) slope. For $\Omega\tau=\pi/2$, differentiating $\theta$ at $\delta=0$ gives $\theta'(0)=1/\Omega$. Consequently the phase near resonance is

$$
\frac{\delta T-\varphi}{2}+\theta
=\frac{\delta T_{\mathrm{eff}}-\varphi}{2}+O[(\delta/\Omega)^3],\qquad
T_{\mathrm{eff}}=T+\frac2\Omega=T+\frac{4\tau}{\pi}.
$$

At $\varphi=\pi/2$ the exact resonant slope is $\partial P/\partial\nu=-\pi T_{\mathrm{eff}}$. For the plotted parameters $T_{\mathrm{eff}}\simeq5.637\,\mathrm{ms}$; the near-resonant estimate $1/(2T_{\mathrm{eff}})\simeq88.71\,\mathrm{Hz}$ explains why the exact finite-pulse width below differs from $100\,\mathrm{Hz}$. The slope is exact at resonance under these assumptions, while this width estimate uses the local phase expansion. A [velocity](velocity.md) distribution requires averaging the full response, not substituting one effective flight time.

## ↑ Ancestors (15)

1. [Finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md)
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
