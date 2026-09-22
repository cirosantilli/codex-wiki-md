# Work in a two-level sudden quench

↑ **Parent:** [Two-level sudden quench](two-level-sudden-quench.md)

The drive can supply or extract [work](work.md) while the [quantum state](quantum-state.md) stays approximately fixed. For a differentiable bounded [Hamiltonian operator](hamiltonian-quantum-mechanics.md), the [Schrödinger equation](schrodinger-equation.md) gives

$$
\frac{d}{dt}\langle H(t)\rangle=\left\langle\frac{\partial H(t)}{\partial t}\right\rangle.
$$

The state-evolution terms cancel, leaving the external drive's [power](power.md). For a finite ideal step the change in mean [energy](energy-split.md) is $\langle\psi|H_f-H_i|\psi\rangle$. Thus [conservation of energy](conservation-of-energy.md) for a closed system with a time-independent [Hamiltonian operator](hamiltonian-quantum-mechanics.md) does not assert conservation of the driven subsystem's [energy](energy-split.md) during switching.

Specify [work](work.md) operationally by two [energy measurements](energy-measurement.md): one before the switch and one after. For the prepared initial [ground state](ground-state.md), the first outcome is definite; the second samples the new [Born rule](born-rule.md) [probabilities](probability.md). This protocol gives a distribution of measured [energy](energy-split.md) differences, rather than generally the measurement distribution of the single operator $H_f-H_i$.[Talkner, Lutz and Hänggi, p. 2, equations (8)–(10): initial energy outcome, conditional transition probability and two-measurement work distribution](fluctuation-theorems-work-is-not-an-observable-by-peter-talkner-and-others.md)

$$
W_g=\frac{\Delta_i-\Delta_f}{2}\quad\hbox{with probability }c^2,\qquad
W_e=\frac{\Delta_i+\Delta_f}{2}\quad\hbox{with probability }s^2,
$$

and hence

$$
\langle H_f\rangle=-\frac{\Delta_f}{2}\cos\theta,\qquad
\langle W\rangle=\frac{\Delta_i-\Delta_f\cos\theta}{2},\qquad
\operatorname{Var}(W)=\frac{\Delta_f^2}{4}\sin^2\theta.
$$

For $\Delta_i=\Delta_f=\Delta$ and $\theta=\pi/3$, the [work](work.md) is $0$ or $\Delta$, with [probabilities](probability.md) $3/4$ and $1/4$; its [expectation](expected-value-split.md) is $\Delta/4$ and its [variance](variance-split.md) is $3\Delta^2/16$. The initial mean [energy](energy-split.md) $-\Delta/2$ becomes $-\Delta/4$. Using different initial and final scalar offsets would also shift the measured [work](work.md); the displayed [Hamiltonian operators](hamiltonian-quantum-mechanics.md) fix that convention explicitly.

## ↑ Ancestors (7)

1. [Two-level sudden quench](two-level-sudden-quench.md)
2. [Quantum quench](quantum-quench.md)
3. [Sudden approximation](sudden-approximation.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
