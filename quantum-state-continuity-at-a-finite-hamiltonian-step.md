# Quantum state continuity at a finite Hamiltonian step

↑ **Parent:** [Sudden approximation](sudden-approximation.md)

For a fixed [Hilbert space](hilbert-space-split.md), a bounded [self-adjoint](self-adjoint-operator.md) [Hamiltonian operator](hamiltonian-quantum-mechanics.md) with a finite step $H_i\to H_f$ at $t=0$ does not deliver an instantaneous rotation of the [quantum state](quantum-state.md). Integrating the [Schrödinger equation](schrodinger-equation.md) across a short interval gives

$$
|\psi(\epsilon)\rangle-|\psi(-\epsilon)\rangle=-\frac{i}{\hbar}\int_{-\epsilon}^{\epsilon}H(t)|\psi(t)\rangle\,dt.
$$

For a normalized [quantum state](quantum-state.md) and $\|H(t)\|\le M$ in [operator norm](operator-norm.md), the difference has [norm](norm.md) at most $2\epsilon M/\hbar$, which tends to zero. The time [derivative](derivative.md) can jump even though the [quantum state](quantum-state.md) is continuous. Here $\hbar$ is the reduced [Planck constant](planck-constant.md). An instantaneous replacement of the [eigenbasis](eigenbasis.md) changes coordinates, not the vector being represented.

For a real switch occupying $0\le t\le\tau$, remove any real scalar contribution $a(t)I$ that produces only a [global phase](global-phase.md), and write $|\widetilde\psi(t)\rangle=e^{i\int_0^t a(s)ds/\hbar}|\psi(t)\rangle$. The same integral argument gives the sufficient bounded-model estimate

$$
\bigl\|\widetilde\psi(\tau)-\psi(0)\bigr\|\le\varepsilon,\qquad
\varepsilon=\frac1\hbar\int_0^\tau\|H(t)-a(t)I\|\,dt.
$$

Thus $\varepsilon\ll1$ controls the [sudden approximation](sudden-approximation.md) up to a [global phase](global-phase.md). For any normalized final [energy eigenstate](energy-eigenstate.md), its [probability amplitude](probability-amplitude.md) differs from the instantaneous-switch value by at most $\varepsilon$, and its [Born rule](born-rule.md) [probability](probability.md) differs by at most $2\varepsilon$. These are sufficient error bounds, not necessary criteria. For the fixed-gap [two-level sudden quench](two-level-sudden-quench.md), any switching path $H(t)=-\Delta\mathbf n(t)\cdot\boldsymbol\sigma/2$ with a unit vector $\mathbf n(t)$ has [operator norm](operator-norm.md) $\Delta/2$, giving $\varepsilon\le\Delta\tau/(2\hbar)$.

This estimate is deliberately for bounded [Hamiltonian operators](hamiltonian-quantum-mechanics.md). An unbounded [energy](energy-split.md) spectrum does not supply a finite global $M$; relevant [quantum states](quantum-state.md), [operator domains](operator-domain.md) and excited [energy eigenvalues](energy-eigenvalue-split.md) require separate control. The [adiabatic theorem](adiabatic-theorem.md) also requires hypotheses about the path and its [spectral gaps](spectral-gap.md); there is no universal switch-duration criterion covering all spectra. The [cold-atom collapse and revival after a lattice quench](cold-atom-collapse-and-revival-after-a-lattice-quench.md) illustrates how a single switch can be sudden for one degree of freedom and slow for another.

**Table of contents**

- [Impulsive quantum kick](impulsive-quantum-kick.md)
  - [Off-diagonal two-state impulse](off-diagonal-two-state-impulse.md)
    - [Time-integrated pulse operator has action units](time-integrated-pulse-operator-has-action-units.md)

## ↑ Ancestors (5)

1. [Sudden approximation](sudden-approximation.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Impulsive quantum kick](impulsive-quantum-kick.md)
- [Sudden approximation](sudden-approximation.md)
