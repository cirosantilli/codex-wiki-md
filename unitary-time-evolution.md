# Unitary time evolution

↑ **Parent:** [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)

A time-independent Hamiltonian evolves a state by the unitary operator $U(t)=e^{-iHt/\hbar}$.

For a closed [quantum system](quantum-system-split.md), [unitary time evolution](unitary-time-evolution.md) changes a [quantum state](quantum-state.md) through a [unitary operator](unitary-operator.md), preserving [norms](norm.md) and [inner products](inner-product-split.md). For a time-independent [self-adjoint](self-adjoint-operator.md) [Hamiltonian operator](hamiltonian-quantum-mechanics.md) $H$, choose the initial time as zero:

$$
i\hbar\frac{d}{dt}|\psi(t)\rangle=H|\psi(t)\rangle,\qquad
|\psi(t)\rangle=U(t)|\psi(0)\rangle,\qquad U(t)=\exp(-iHt/\hbar).
$$

Here $\hbar=h/(2\pi)$ is the reduced [Planck constant](planck-constant.md). The same $U(t)$ acts on every initial [quantum state](quantum-state.md); it depends on the [Hamiltonian operator](hamiltonian-quantum-mechanics.md) and elapsed time, rather than the chosen preparation.[Quantum Physics II (8.05), Fall 2013; Zwiebach, Quantum Dynamics, sections 2.1 and 2.3, printed pp. 10–11 and 15–16, equations (2.3), (2.6)–(2.7) and (2.45)](quantum-physics-ii-8-05-fall-2013/quantum-dynamics.md)

The [self-adjointness](self-adjoint-operator.md) of $H$ makes the exponential a [unitary operator](unitary-operator.md). In finite [dimension](dimension-vector-space.md), conjugating its [matrix exponential](matrix-exponential.md) gives

$$
U(t)^\dagger=\exp(iHt/\hbar)=U(-t),\qquad
U(t)^\dagger U(t)=UU^\dagger=I.
$$

The two exponents commute because both are multiples of $H$. Hence, for any two initial [vectors](vector.md),

$$
\langle U\phi|U\psi\rangle=\langle\phi|U^\dagger U|\psi\rangle
=\langle\phi|\psi\rangle,\qquad \|U\psi\|=\|\psi\|.
$$

This short proof explains why normalization survives, why [orthogonality](orthogonal-vectors.md) of initial [vectors](vector.md) survives, and why the [transition probability](transition-probability.md) between two states evolved by the same $U$ is unchanged. It does not require that a fixed [measurement in quantum mechanics](quantum-measurement-split.md) have time-independent [probabilities](probability.md): its measurement [basis](basis.md) need not move with the [quantum states](quantum-state.md).

For an unbounded [self-adjoint operator](self-adjoint-operator.md), define the exponential through the [spectral theorem](spectral-theorem.md), rather than assuming that its power series acts on every [vector](vector.md). It is a [unitary operator](unitary-operator.md) on the entire [Hilbert space](hilbert-space-split.md); the strong [Schrödinger equation](schrodinger-equation.md) holds for initial [vectors](vector.md) in the [operator domain](operator-domain.md) $D(H)$. For a [density operator](density-matrix-split.md), [unitary time evolution](unitary-time-evolution.md) reads $\rho(t)=U(t)\rho(0)U(t)^\dagger$. It preserves [eigenvalues](eigenvalue.md) and [purity of a density operator](purity-of-a-density-operator.md), but can change its entries in a fixed [basis](basis.md).

The useful distinction is between conserving total [probability](probability.md) and conserving each measurement's [probabilities](probability.md). A fixed [energy](energy-split.md) spectrum supplies different ticking rates for different [probability amplitudes](probability-amplitude.md). Their relative [quantum phases](quantum-phase.md) can move the [Bloch vector](bloch-vector.md) and create [quantum interference](quantum-interference.md) even while every [energy eigenstate](energy-eigenstate.md) population stays fixed. [Qubit precession under a constant Hamiltonian](qubit-precession-under-a-constant-hamiltonian.md) makes this visible; [Ramsey interferometry](ramsey-interferometry.md) converts the accumulated relative [quantum phase](quantum-phase.md) into a population difference that a simple readout can detect.

**Table of contents**

- [Perfect quantum state transfer](perfect-quantum-state-transfer.md)
- [Schrödinger picture](schrodinger-picture.md)
- [Time-evolution operator](time-evolution-operator.md)
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
- [Quantum-mechanical propagator](quantum-mechanical-propagator.md)
  - [Quantum-mechanical propagator in a constant force](quantum-mechanical-propagator-in-a-constant-force.md)
    - [Momentum-space propagator in a uniform force](momentum-space-propagator-in-a-uniform-force.md)
  - [Normalized short-time Schrödinger kernel](normalized-short-time-schrodinger-kernel.md)
    - [Schrödinger equation from a short-time path integral](schrodinger-equation-from-a-short-time-path-integral.md)
  - [Free-particle propagator](free-particle-propagator.md)
    - [Fresnel convolution of free-particle time slices](fresnel-convolution-of-free-particle-time-slices.md)
    - [Euclidean free-particle bridge amplitude](euclidean-free-particle-bridge-amplitude.md)
  - [Semiclassical propagator](semiclassical-propagator.md)
    - [Dirichlet fluctuation determinant of a semiclassical propagator](dirichlet-fluctuation-determinant-of-a-semiclassical-propagator.md)
    - [Van Vleck determinant](van-vleck-determinant.md)
- [Heisenberg picture](heisenberg-picture.md)
  - [Heisenberg equation of motion](heisenberg-equation-of-motion.md)
- [Interaction picture](interaction-picture.md)
- [Time-reversal symmetry in quantum mechanics](time-reversal-symmetry-in-quantum-mechanics.md)
  - [Quantum time-reversal operator](quantum-time-reversal-operator.md)
  - [Unitary time reversal reverses the energy spectrum](unitary-time-reversal-reverses-the-energy-spectrum.md)
  - [Antiunitary time reversal preserves the energy spectrum](antiunitary-time-reversal-preserves-the-energy-spectrum.md)
- [Rabi cycle](rabi-cycle.md)
  - [Rotating-frame Rabi Hamiltonian](rotating-frame-rabi-hamiltonian.md)
  - [Circularly rotating magnetic drive](circularly-rotating-magnetic-drive.md)
  - [Rabi frequency](rabi-frequency.md)
  - [Resonance envelope of a Rabi transition](resonance-envelope-of-a-rabi-transition.md)
  - [Driven two-level Rabi model](driven-two-level-rabi-model.md)
    - [Rabi vector](rabi-vector.md)
    - [Equatorial reachability of a detuned spin pulse](equatorial-reachability-of-a-detuned-spin-pulse.md)
    - [Laboratory phase of a resonant spin pulse](laboratory-phase-of-a-resonant-spin-pulse.md)
    - [Rabi angular frequency](rabi-angular-frequency.md)
    - [Rabi detuning](rabi-detuning.md)
    - [Rabi pi pulse](rabi-pi-pulse.md)
  - [Rabi molecular beam magnetic resonance experiment](rabi-molecular-beam-magnetic-resonance-experiment.md)
    - [Rabi transit-time and field averaging](rabi-transit-time-and-field-averaging.md)

## ↑ Ancestors (8)

1. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
2. [Observable](observable.md)
3. [Quantum state](quantum-state.md)
4. [Quantum system](quantum-system-split.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (54)

- [Ghirardi-Rimini-Weber theory](ghirardi-rimini-weber-theory.md)
- [Hadamard-phase-Hadamard qubit rotation](hadamard-phase-hadamard-qubit-rotation.md)
- [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
- [Impulsive quantum kick](impulsive-quantum-kick.md)
- [One-sided sudden expansion of an infinite square well](one-sided-sudden-expansion-of-an-infinite-square-well.md)
- [Operator exponential](operator-exponential.md)
- [Operator support](operator-support.md)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/20f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/20f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-62/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/16b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57/4/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/31a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-50/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/15b/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/34a/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/34b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/15b/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-325/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325/1/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-c/c11/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-b/b6/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-b/b7/d/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-d/d9/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2013/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1/1/a/solution.md)
- [Post-quench oscillations in a two-level system](post-quench-oscillations-in-a-two-level-system.md)
- [Quantum phase estimation with a maximally mixed target](quantum-phase-estimation-with-a-maximally-mixed-target.md)
- [Quantum quench](quantum-quench.md)
- [Quantum time-reversal operator](quantum-time-reversal-operator.md)
- [Rabi cycle](rabi-cycle.md)
- [Schrödinger equation](schrodinger-equation.md)
- [Spectral filtering of Hamiltonian terms](spectral-filtering-of-hamiltonian-terms.md)
- [Sudden approximation](sudden-approximation.md)
- [Time evolution](time-evolution.md)
- [Time-evolution operator](time-evolution-operator.md)
- [Trapped-ion sideband pulse model](trapped-ion-sideband-pulse-model.md)
- [Two-level observable transition probability](two-level-observable-transition-probability.md)
- [Two-level quantum return probability](two-level-quantum-return-probability.md)
- [Unitary time evolution](unitary-time-evolution.md)
- [Zurek spin-bath model](zurek-spin-bath-model.md)
