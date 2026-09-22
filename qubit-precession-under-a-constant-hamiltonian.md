# Qubit precession under a constant Hamiltonian

↑ **Parent:** [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)

Choose the [Pauli matrices](pauli-matrices.md) with $\sigma_z=\operatorname{diag}(1,-1)$, and let $\omega>0$ be an [angular frequency](angular-frequency.md). The [computational basis](computational-basis.md) is an [orthonormal basis](orthonormal-basis.md) of [energy eigenstates](energy-eigenstate.md) for the [qubit](qubit.md) [Hamiltonian operator](hamiltonian-quantum-mechanics.md)

$$
H=\frac{\hbar\omega}{2}\sigma_z,\qquad
E_0=\frac{\hbar\omega}{2},\quad E_1=-\frac{\hbar\omega}{2},\qquad
U(t)=\begin{pmatrix}e^{-i\omega t/2}&0\\0&e^{i\omega t/2}\end{pmatrix}.
$$

In this convention $|1\rangle$ is the lower [energy eigenstate](energy-eigenstate.md); the labels describe a [basis](basis.md) choice, not a universal [ground state](ground-state.md)/[excited state](excited-state.md) ordering. Start in the [Hadamard basis](hadamard-basis.md) [pure state](pure-state.md) $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$. Then

$$
|\psi(t)\rangle=\frac{e^{-i\omega t/2}|0\rangle+e^{i\omega t/2}|1\rangle}{\sqrt2}
=e^{-i\omega t/2}\frac{|0\rangle+e^{i\omega t}|1\rangle}{\sqrt2},\qquad
\rho(t)=\frac12\begin{pmatrix}1&e^{-i\omega t}\\e^{i\omega t}&1\end{pmatrix}.
$$

The first factor in the second expression is a [global phase](global-phase.md). The ratio of the two [probability amplitudes](probability-amplitude.md) has relative [quantum phase](quantum-phase.md) $\omega t$, so its sign follows directly from $E_1-E_0=-\hbar\omega$.

Multiplying this [density matrix](density-matrix-split.md) by each [Pauli matrix](pauli-matrices.md) and taking its [trace](matrix-trace.md) gives the [Bloch vector](bloch-vector.md):

$$
\langle\sigma_x\rangle_t=\cos(\omega t),\qquad
\langle\sigma_y\rangle_t=\sin(\omega t),\qquad
\langle\sigma_z\rangle_t=0.
$$

The [Bloch vector](bloch-vector.md) travels counterclockwise around the equator of the [Bloch sphere](bloch-sphere.md), from $+x$ toward $+y$ when viewed from $+z$. A [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) always has $P_Z(0)=P_Z(1)=1/2$, while the [Hadamard basis](hadamard-basis.md) and $\sigma_y$ [eigenbasis](eigenbasis.md) measurements give

$$
P_X(+)=\frac{1+\cos(\omega t)}2,\qquad
P_Y(+)=\frac{1+\sin(\omega t)}2.
$$

At $\omega t=\pi/2$, the [quantum state](quantum-state.md) is $|+i\rangle=(|0\rangle+i|1\rangle)/\sqrt2$ up to a [global phase](global-phase.md), giving $P_Y(+)=1$. At $\omega t=\pi$, it is $|-\rangle$ up to a [global phase](global-phase.md), giving $P_X(+)=0$. Both retain equal [energy measurement](energy-measurement.md) [probabilities](probability.md).

<a id="image-relative-phase-rotates-a-qubit-while-energy-populations-stay-fixed"></a>
![](unitary-qubit-precession.png)

**[Figure 7](#image-relative-phase-rotates-a-qubit-while-energy-populations-stay-fixed). Relative phase rotates a qubit while energy populations stay fixed**. Original ideal-model equatorial Bloch-vector diagram and exact Born-rule probabilities for $H=\hbar\omega\sigma_z/2$ and initial $|+\rangle$. The horizontal variable is the dimensionless phase $\omega t$; no curve is measured data.

At $t=2\pi/\omega$, the [time-evolution operator](time-evolution-operator.md) is $U(t)=-I$, so $|\psi(t)\rangle=-|+\rangle$. The physical [quantum state ray](quantum-state-ray.md), its [density operator](density-matrix-split.md), and every measurement's [probabilities](probability.md) have returned. The representative [vector](vector.md) returns exactly only at $t=4\pi/\omega$, when $U(t)=I$. The minus sign is a [global phase](global-phase.md) for this isolated evolution; comparing an evolved branch with an unevolved branch through a [controlled unitary gate](controlled-unitary-gate.md) can make it a relative [quantum phase](quantum-phase.md), as explained in [global phase of an uncontrolled quantum gate is unobservable](global-phase-of-an-uncontrolled-quantum-gate-is-unobservable.md).

**Table of contents**

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

## ↑ Ancestors (11)

1. [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)
2. [Time-evolution operator](time-evolution-operator.md)
3. [Unitary time evolution](unitary-time-evolution.md)
4. [Hamiltonian (quantum mechanics)](hamiltonian-quantum-mechanics.md)
5. [Observable](observable.md)
6. [Quantum state](quantum-state.md)
7. [Quantum system](quantum-system-split.md)
8. [Quantum mechanics](quantum-mechanics-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Unitary time evolution](unitary-time-evolution.md)
