<h1 id="section-d/d9/solution">Solution</h1>

↑ **Parent:** [D9](../d9.md)

Time dependence in [quantum mechanics](../../../../../quantum-mechanics-split.md) describes how a prepared [quantum state](../../../../../quantum-state.md) changes and thereby changes the [probabilities](../../../../../probability.md) of later measurements. For an isolated system, the [Schrödinger picture](../../../../../schrodinger-picture.md) assigns this evolution to a state vector $|\psi(t)\rangle$, governed by the [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md)

$$
i\hbar\frac{d}{dt}|\psi(t)\rangle=\hat H(t)|\psi(t)\rangle.
$$

The [Hamiltonian](../../../../../hamiltonian.md) is a [self-adjoint operator](../../../../../self-adjoint-operator.md); it has units of [energy](../../../../../energy-split.md), while $\hbar$ has units of [action](../../../../../action.md), so $\hat H/\hbar$ has units of inverse time. For a particle with [potential energy](../../../../../potential-energy.md) $V(\mathbf r,t)$, this becomes

$$
i\hbar\partial_t\psi(\mathbf r,t)
=\left[-\frac{\hbar^2}{2m}\nabla^2+V(\mathbf r,t)\right]\psi(\mathbf r,t).
$$

Given a suitable initial [wavefunction](../../../../../wave-function-split.md) and the physical [boundary conditions](../../../../../boundary-condition.md), this first-order equation determines its subsequent propagation. Its [linearity](../../../../../linearity.md) means that the evolution of a [quantum superposition](../../../../../quantum-superposition.md) is the corresponding [quantum superposition](../../../../../quantum-superposition.md) of evolved states.

For a real [potential energy](../../../../../potential-energy.md), this equation and its [complex conjugate](../../../../../complex-conjugate.md) imply the local [continuity equation](../../../../../continuity-equation.md)

$$
\partial_t\rho+\nabla\cdot\mathbf j=0,
\qquad \rho=|\psi|^2,
\qquad \mathbf j=\frac{\hbar}{m}\operatorname{Im}(\psi^*\nabla\psi).
$$

Here $\rho$ is the [probability density](../../../../../probability-density.md) and $\mathbf j$ the [probability current](../../../../../probability-current.md). Vanishing net boundary flux preserves [wavefunction normalization](../../../../../wavefunction-normalization.md), as required by the [Born rule](../../../../../born-rule.md).

The [time-evolution operator](../../../../../time-evolution-operator.md) packages the solution for every initial state:

$$
|\psi(t)\rangle=U(t,t_0)|\psi(t_0)\rangle,
\qquad i\hbar\partial_tU(t,t_0)=\hat H(t)U(t,t_0),
\qquad U(t_0,t_0)=I.
$$

Because $\hat H^\dagger=\hat H$, differentiation gives

$$
\frac d{dt}(U^\dagger U)
=\frac i\hbar U^\dagger\hat H U-\frac i\hbar U^\dagger\hat H U=0.
$$

Therefore $U^\dagger U=I$: this is [unitary time evolution](../../../../../unitary-time-evolution.md), preserving [inner products](../../../../../inner-product-split.md) and all state [norms](../../../../../norm.md). It is reversible, with $U(t,t_0)^{-1}=U(t_0,t)=U(t,t_0)^\dagger$, and obeys the composition law $U(t_2,t_0)=U(t_2,t_1)U(t_1,t_0)$.

For a time-independent [Hamiltonian](../../../../../hamiltonian.md), the solution is the [operator exponential](../../../../../operator-exponential.md)

$$
\boxed{U(t,t_0)=\exp[-i\hat H(t-t_0)/\hbar].}
$$

If the [Hamiltonian](../../../../../hamiltonian.md) varies with time, the analogous simple exponential of its integral is valid when $[\hat H(t),\hat H(t')]=0$ for all relevant times. Otherwise [time ordering](../../../../../time-ordering.md) is essential:

$$
U(t,t_0)=\mathcal T\exp\left[-\frac i\hbar\int_{t_0}^t\hat H(t')\,dt'\right].
$$

The meaning is explicit in the first terms of the ordered series,

$$
U=I-\frac i\hbar\int_{t_0}^t\hat H(t_1)\,dt_1
-\frac1{\hbar^2}\int_{t_0}^t dt_1\int_{t_0}^{t_1}dt_2\,\hat H(t_1)\hat H(t_2)+\cdots:
$$

the later-time operator stands on the left. In the position representation, the same propagation is expressed by the [quantum-mechanical propagator](../../../../../quantum-mechanical-propagator.md)

$$
K(\mathbf r,t;\mathbf r',t_0)=\langle\mathbf r|U(t,t_0)|\mathbf r'\rangle,
\qquad
\psi(\mathbf r,t)=\int K(\mathbf r,t;\mathbf r',t_0)\psi(\mathbf r',t_0)\,d^3r'.
$$

Its initial value is the [Dirac delta function](../../../../../dirac-delta-function.md) $\delta^3(\mathbf r-\mathbf r')$.

A time-independent [Hamiltonian](../../../../../hamiltonian.md) has [energy eigenstates](../../../../../energy-eigenstate.md) satisfying $\hat H|n\rangle=E_n|n\rangle$. A single such initial state evolves as

$$
|\psi_n(t)\rangle=e^{-iE_n(t-t_0)/\hbar}|n\rangle.
$$

It is a [stationary state](../../../../../stationary-state.md): its [global phase](../../../../../global-phase.md) changes, but its [probability density](../../../../../probability-density.md) and the distributions of time-independent [observables](../../../../../observable.md) do not. Its [energy](../../../../../energy-split.md) is sharp. Any [quantum superposition](../../../../../quantum-superposition.md) entirely within one degenerate [energy eigenspace](../../../../../energy-eigenspace.md) also acquires one common [global phase](../../../../../global-phase.md) and is stationary. Stationarity does not require zero [probability current](../../../../../probability-current.md); for instance, $u_n(\phi)=e^{in\phi}/\sqrt{2\pi}$ on the ring has a constant density and persistent circulation when $n\ne0$.

An arbitrary normalized state can instead contain different [energy eigenvalues](../../../../../energy-eigenvalue-split.md):

$$
|\psi(t)\rangle=\sum_n c_ne^{-iE_n(t-t_0)/\hbar}|n\rangle,
\qquad \sum_n|c_n|^2=1.
$$

A [continuous spectrum](../../../../../continuous-spectrum.md) requires corresponding integrals. For the discrete case, an [energy measurement](../../../../../energy-measurement.md) gives $E_n$ with fixed [probability](../../../../../probability.md) $|c_n|^2$ (summed over degeneracies), but relative [quantum phases](../../../../../quantum-phase.md) change with time. Consequently

$$
|\psi(\mathbf r,t)|^2=\sum_{m,n}c_m^*c_n\phi_m^*(\mathbf r)\phi_n(\mathbf r)
 e^{i(E_m-E_n)(t-t_0)/\hbar}.
$$

The [interference](../../../../../interference-wave-propagation.md) terms can oscillate at [angular frequencies](../../../../../angular-frequency.md) $(E_m-E_n)/\hbar$. For two populated [energy levels](../../../../../energy-level.md), this supplies a characteristic period $2\pi\hbar/|E_m-E_n|$ when the [interference](../../../../../interference-wave-propagation.md) term is nonzero. Thus fixed energy populations do not imply a stationary spatial distribution.

For a normalized state and an [observable](../../../../../observable.md) $\hat A(t)$, its [expectation value](../../../../../expectation-value.md) is

$$
\langle A\rangle_t=\langle\psi(t)|\hat A(t)|\psi(t)\rangle.
$$

This is the statistical [mean](../../../../../expected-value-split.md) over repeated preparations and measurements. In an [eigenbasis](../../../../../eigenbasis.md) of [energy eigenstates](../../../../../energy-eigenstate.md) for a time-independent [Hamiltonian](../../../../../hamiltonian.md) and a time-independent $\hat A$,

$$
\langle A\rangle_t=\sum_{m,n}c_m^*c_n A_{mn}e^{i(E_m-E_n)(t-t_0)/\hbar}.
$$

Only [matrix elements](../../../../../matrix-element.md) connecting different [energies](../../../../../energy-split.md) can generate these oscillations. If $[\hat A,\hat H]=0$, its [expectation value](../../../../../expectation-value.md) is constant for every initial state, provided it has no explicit time dependence.

Differentiating the [expectation value](../../../../../expectation-value.md) and substituting the [Schrödinger equation](../../../../../schrodinger-equation.md) for both the bra and ket proves the general [Ehrenfest theorem](../../../../../ehrenfest-theorem.md):

$$
\begin{aligned}
\frac d{dt}\langle A\rangle
&=\langle\dot\psi|\hat A|\psi\rangle+
\left\langle\frac{\partial\hat A}{\partial t}\right\rangle+
\langle\psi|\hat A|\dot\psi\rangle\\
&=\frac i\hbar\langle\hat H\hat A-\hat A\hat H\rangle+
\left\langle\frac{\partial\hat A}{\partial t}\right\rangle.
\end{aligned}
$$

Equivalently,

$$
\boxed{\frac d{dt}\langle A\rangle
=\frac1{i\hbar}\langle[\hat A,\hat H]\rangle+
\left\langle\frac{\partial\hat A}{\partial t}\right\rangle.}
$$

These manipulations require the state to lie in the relevant [operator domains](../../../../../operator-domain.md). Taking $\hat A=\hat H$ gives $d\langle H\rangle/dt=\langle\partial_t\hat H\rangle$, so [energy](../../../../../energy-split.md) is conserved under a time-independent [Hamiltonian](../../../../../hamiltonian.md).

For $\hat H=\hat p^2/(2m)+V(\hat x)$, the [canonical commutation relation](../../../../../canonical-commutation-relation.md) gives

$$
[\hat x,\hat H]=\frac{i\hbar}{m}\hat p,
\qquad [\hat p,\hat H]=-i\hbar V'(\hat x).
$$

Hence the particularly useful position-and-momentum form of [Ehrenfest theorem](../../../../../ehrenfest-theorem.md) is

$$
\boxed{\frac d{dt}\langle x\rangle=\frac{\langle p\rangle}{m},
\qquad \frac d{dt}\langle p\rangle=-\langle V'(x)\rangle.}
$$

It resembles [Newton's second law](../../../../../newton-s-second-law.md), but the mean [force](../../../../../force-split.md) generally differs from the [force](../../../../../force-split.md) at the mean position. If a narrow [wave packet](../../../../../wave-packet.md) samples a region where the [force](../../../../../force-split.md) varies little, $\langle V'(x)\rangle\simeq V'(\langle x\rangle)$ gives approximate classical motion. For a quadratic [potential energy](../../../../../potential-energy.md) this replacement is exact. In particular the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) obeys

$$
\frac{d^2}{dt^2}\langle x\rangle=-\omega^2\langle x\rangle,
\qquad
\langle x\rangle_t=\langle x\rangle_{t_0}\cos\omega\tau+
\frac{\langle p\rangle_{t_0}}{m\omega}\sin\omega\tau,
\qquad \tau=t-t_0.
$$

The centroid follows the classical [harmonic oscillator](../../../../../simple-harmonic-motion.md), although this does not specify the full evolving [wavefunction](../../../../../wave-function-split.md) or its width.

The [Heisenberg picture](../../../../../heisenberg-picture.md) expresses the same physics by assigning evolution to [observables](../../../../../observable.md) instead:

$$
\hat A_H(t)=U^\dagger(t,t_0)\hat A_S(t)U(t,t_0),
\qquad |\psi_H\rangle=|\psi(t_0)\rangle.
$$

The [expectation value](../../../../../expectation-value.md) is unchanged, and differentiation yields $d\hat A_H/dt=(i/\hbar)[\hat H_H,\hat A_H]+U^\dagger(\partial_t\hat A_S)U$. Thus state propagation, evolving [expectation values](../../../../../expectation-value.md), and the classical correspondence in [Ehrenfest theorem](../../../../../ehrenfest-theorem.md) are mutually consistent descriptions of the same [unitary time evolution](../../../../../unitary-time-evolution.md).

## ↑ Ancestors (14)

1. [D9](../d9.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
