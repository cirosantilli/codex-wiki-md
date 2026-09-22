# Time-evolution operator

↑ **Parent:** [Unitary time evolution](unitary-time-evolution.md)

The time-evolution operator maps an initial [quantum state](quantum-state.md) to its state at a later time. For a time-independent [Hamiltonian operator](hamiltonian-quantum-mechanics.md) $H$, it is the [unitary operator](unitary-operator.md) $U(t)=e^{-iHt/\hbar}$.

More generally, write $|\psi(t)\rangle=U(t,t_0)|\psi(t_0)\rangle$. The [time-evolution operator](time-evolution-operator.md) obeys

$$
U(t_0,t_0)=I,\qquad U(t_2,t_0)=U(t_2,t_1)U(t_1,t_0),\qquad
U(t,t_0)^{-1}=U(t,t_0)^\dagger=U(t_0,t).
$$

For a constant [self-adjoint](self-adjoint-operator.md) [Hamiltonian operator](hamiltonian-quantum-mechanics.md), $U(t,t_0)=\exp[-iH(t-t_0)/\hbar]$. With zero as the initial time, this gives the group law $U(t+s)=U(t)U(s)$. Successive evolution is reversible; a measurement followed by conditioning on an outcome is a separate operation described by [projective measurement](projective-measurement.md).

For a time-dependent [Hamiltonian operator](hamiltonian-quantum-mechanics.md), the defining equation is $i\hbar\partial_tU(t,t_0)=H(t)U(t,t_0)$. In finite [dimension](dimension-vector-space.md), a continuous [Hermitian](hermitian-operator.md) $H(t)$ still gives [unitary time evolution](unitary-time-evolution.md), since

$$
\frac{d}{dt}(U^\dagger U)
=\frac{i}{\hbar}U^\dagger H(t)U-\frac{i}{\hbar}U^\dagger H(t)U=0.
$$

The solution is a [time-ordered exponential](time-ordered-exponential.md), with later factors acting on the left. One may replace it by $\exp[-i\int_{t_0}^tH(s)\,ds/\hbar]$ when $[H(s),H(s')]=0$ at all times; independently changing pulse axes generally requires [time ordering](time-ordering.md).[Quantum Physics II (8.05), Fall 2013; Zwiebach, Quantum Dynamics, section 2.3, printed pp. 16–17, equations (2.46)–(2.52) and Case 3](quantum-physics-ii-8-05-fall-2013/quantum-dynamics.md)

**Table of contents**

- [Quantum propagator](quantum-propagator.md)
  - [Spectral resolution of a quantum propagator](spectral-resolution-of-a-quantum-propagator.md)
- [Floquet operator](floquet-operator.md)
  - [Delta-kicked spin Floquet operator](delta-kicked-spin-floquet-operator.md)
  - [Pulse-and-precession spin one-half map](pulse-and-precession-spin-one-half-map.md)
  - [Quasienergy](quasienergy.md)
- [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)
  - [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md)
    - [Ramsey interferometry](ramsey-interferometry.md)
      - [Initial-state dependence of Ramsey contrast](initial-state-dependence-of-ramsey-contrast.md)
      - [Ramsey ensemble coherence](ramsey-ensemble-coherence.md)
      - [Quantronium Ramsey interference experiment](quantronium-ramsey-interference-experiment.md)
      - [Ramsey separated oscillatory fields experiment](ramsey-separated-oscillatory-fields-experiment.md)
        - [Ramsey spectroscopy](ramsey-spectroscopy.md)
          - [Ramsey frequency precision](ramsey-frequency-precision.md)
        - [Finite-pulse Ramsey transition probability](finite-pulse-ramsey-transition-probability.md)
          - [Ramsey fringe envelope](ramsey-fringe-envelope.md)
          - [Finite-pulse Ramsey phase response](finite-pulse-ramsey-phase-response.md)
          - [Velocity-averaged Ramsey line](velocity-averaged-ramsey-line.md)

## ↑ Ancestors (9)

1. [Unitary time evolution](unitary-time-evolution.md)
2. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
3. [Observable](observable.md)
4. [Quantum state](quantum-state.md)
5. [Quantum system](quantum-system-split.md)
6. [Quantum mechanics](quantum-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2022/section-b/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-62/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/32d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-63/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-48/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/33b/b/ii/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-d/d9/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge/2013/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2012/paper-1/5/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2014/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017/3/a/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2019/1/c/solution.md)
- [Position eigenstate](position-eigenstate.md)
- [Quantum propagator](quantum-propagator.md)
- [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md)
- [Spectral resolution of a quantum propagator](spectral-resolution-of-a-quantum-propagator.md)
- [Time-evolution operator](time-evolution-operator.md)
