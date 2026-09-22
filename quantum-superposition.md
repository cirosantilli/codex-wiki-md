# Quantum superposition

↑ **Parent:** [Quantum state](quantum-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_superposition)

A quantum superposition is a [linear combination](linear-combination.md) of [quantum state](quantum-state.md) vectors in a complex [Hilbert space](hilbert-space-split.md). In a specified [orthonormal basis](orthonormal-basis.md), a normalized [pure state](pure-state.md) has the displayed expansion, where $a_j$ are [probability amplitudes](probability-amplitude.md). A nonzero [linear combination](linear-combination.md) can always be normalized; an arbitrary sum of normalized vectors need not already have [norm](norm.md) one. Having more than one nonzero component depends on the chosen [basis](basis.md): the [Hadamard basis](hadamard-basis.md) vector $|+\rangle$ is a [quantum superposition](quantum-superposition.md) of the two [computational-basis states](computational-basis-state.md), but is a single vector of the [Hadamard basis](hadamard-basis.md). [Zwiebach, MIT 8.04, lecture 1, section 4, pp. 10–12](https://ocw.mit.edu/courses/8-04-quantum-physics-i-spring-2016/7f930e013cef9cd7dec5aa88baa83f0a_MIT8_04S16_LecNotes1.pdf).

The distinction from classical ignorance is quantitative. Consider the normalized [qubit](qubit.md) [quantum state](quantum-state.md)

$$
|\psi_\phi\rangle=\frac{\sqrt3}{2}|0\rangle+\frac{e^{i\phi}}2|1\rangle.
$$

Its [density operator](density-matrix-split.md), written in the [computational basis](computational-basis.md), is

$$
\rho_\phi=|\psi_\phi\rangle\langle\psi_\phi|
=\begin{pmatrix}3/4&(\sqrt3/4)e^{-i\phi}\\(\sqrt3/4)e^{i\phi}&1/4\end{pmatrix}.
$$

Preparing $|0\rangle$ with [probability](probability.md) $3/4$ and $|1\rangle$ with [probability](probability.md) $1/4$, while discarding the preparation label, instead gives the [mixed state](mixed-state.md)

$$
\rho_{\mathrm{mix}}=\frac34|0\rangle\langle0|+\frac14|1\rangle\langle1|
=\begin{pmatrix}3/4&0\\0&1/4\end{pmatrix}.
$$

The diagonal entries agree, so both preparations give the same [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) [probabilities](probability.md). The off-diagonal entries of $\rho_\phi$ retain [quantum coherence](quantum-coherence-in-a-specified-basis.md) and the relative [quantum phase](quantum-phase.md). In the [Hadamard basis](hadamard-basis.md), the [Born rule](born-rule.md) gives

$$
\langle\pm|\rho_{\mathrm{mix}}|\pm\rangle=\frac12,
\qquad
\langle\pm|\rho_\phi|\pm\rangle=\frac12\pm\frac{\sqrt3}{4}\cos\phi.
$$

The [density matrix](density-matrix-split.md) representation retains this distinction between a [pure state](pure-state.md) and a [mixed state](mixed-state.md). [Watrous, IBM Quantum Learning, Density matrix basics, Interpretation of density matrices and Connection to quantum state vectors](https://quantum.cloud.ibm.com/learning/en/courses/general-formulation-of-quantum-information/density-matrices/density-matrix-basics).

For example, at $\phi=0$, the [quantum superposition](quantum-superposition.md) yields the plus outcome with [probability](probability.md) about $0.9330$, whereas the [mixed state](mixed-state.md) yields it with [probability](probability.md) $0.5$. At $\phi=\pi/2$ these particular [probabilities](probability.md) agree, although the [density matrices](density-matrix-split.md) still differ: equality for one measurement does not establish equality of [quantum states](quantum-state.md). The [probability amplitude](probability-amplitude.md) figure shows the comparison throughout a full cycle of relative [quantum phase](quantum-phase.md).

This is why a [quantum superposition](quantum-superposition.md) is useful: [quantum gates](quantum-logic-gate.md) act linearly on its [probability amplitudes](probability-amplitude.md), and [unitary operators](unitary-operator.md) preserve the full [pure state](pure-state.md) information, including relative [quantum phases](quantum-phase.md). A [Hadamard gate](hadamard-gate.md) can turn otherwise hidden [quantum coherence](quantum-coherence-in-a-specified-basis.md) into different outcome [probabilities](probability.md). The beautiful feature is that the same basis weights can support different predictions when amplitudes recombine. The expansion specifies a preparation and its measurement predictions; it does not assign every unmeasured outcome a simultaneous classical value. See [projective measurement](projective-measurement.md) for the separate question of the conditional state after a measurement.

**Table of contents**

- [Quantum interference](quantum-interference.md)
  - [Period of two-state quantum interference](period-of-two-state-quantum-interference.md)
  - [Hong-Ou-Mandel effect](hong-ou-mandel-effect.md)

## ↑ Ancestors (6)

1. [Quantum state](quantum-state.md)
2. [Quantum system](quantum-system-split.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (78)

- [Amplitude amplification](amplitude-amplification.md)
- [Born rule](born-rule.md)
- [Driven two-level Rabi model](driven-two-level-rabi-model.md)
- [Electron shelving](electron-shelving.md)
- [Elitzur-Vaidman bomb tester](elitzur-vaidman-bomb-tester.md)
- [Energy eigenspace](energy-eigenspace.md)
- [Energy eigenstate](energy-eigenstate.md)
- [Energy populations and evolving relative phases](energy-populations-and-evolving-relative-phases.md)
- [Erwin Schrödinger](erwin-schrodinger.md)
- [Excited state](excited-state.md)
- [Exclusion versus particle position](exclusion-versus-particle-position.md)
- [Finite oscillator commutator boundary defect](finite-oscillator-commutator-boundary-defect.md)
- [Function oracle](function-oracle.md)
- [Ground-state degeneracy](ground-state-degeneracy.md)
- [Hadamard-conjugated linear oracle](hadamard-conjugated-linear-oracle.md)
- [Harmonic-oscillator number-state second moments](harmonic-oscillator-number-state-second-moments.md)
- [Haroche cavity photon nondemolition experiment](haroche-cavity-photon-nondemolition-experiment.md)
- [Infinite square well](infinite-square-well.md)
- [Interaction eigenstate](interaction-eigenstate.md)
- [Mixed state](mixed-state.md)
- [Nondegenerate phase-flip correction in the Steane code](nondegenerate-phase-flip-correction-in-the-steane-code.md)
- [Parity computation by CNOT gates](parity-computation-by-cnot-gates.md)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1/1/solution.md)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2024/paper-1/a1/b/iv/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/quantum-information/1/f/ii/solution.md)
- [Solution](past-exam-of-the-field-theories-and-collective-phenomena-in-condensed-matter-course-of-the-university-of-oxford/2025/3/d/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8/7/2/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8/8/2/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2006/5/1/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2008/8/1/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/8/2/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2017/3/c/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2019/3/e/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2019/6/d/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2021/4/c/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2021/4/d/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2021/4/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/a/solution.md)
- [Solution](past-exam-of-the-nonlinear-optics-and-quantum-states-of-light-course-of-the-university-of-cambridge/2015/paper-1/3/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-2/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-b/b8/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-b/b7/d/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-b/b7/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2022/paper-1/section-d/d9/solution.md)
- [Solution](past-exam-of-the-quantum-physics-course-of-the-university-of-oxford/2016/6/a/solution.md)
- [Solution](past-exam-of-the-quantum-theory-course-of-the-university-of-oxford/2015/1/a/iii/solution.md)
- [Solution](past-exam-of-the-quantum-theory-course-of-the-university-of-oxford/2023/3/c/i/solution.md)
- [Solution](past-exam-of-the-short-options-paper-of-the-physics-prelims-of-the-university-of-oxford/2022/s03/2/c/solution.md)
- [Solution](past-exam-of-the-short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2012/s3/3/4/solution.md)
- [Solution](past-exam-of-the-short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2015/s3/3/4/solution.md)
- [Photon-number measurement backaction](photon-number-measurement-backaction.md)
- [Polarization preparation and dephasing experiment](polarization-preparation-and-dephasing-experiment.md)
- [Probability amplitude](probability-amplitude.md)
- [Quadratic excitation of an oscillator ground state](quadratic-excitation-of-an-oscillator-ground-state.md)
- [Quantum error correction](quantum-error-correction-split.md)
- [Quantum mechanics](quantum-mechanics-split.md)
- [Quantum state](quantum-state.md)
- [Quantum superposition](quantum-superposition.md)
- [Quark-model constituent bookkeeping](quark-model-constituent-bookkeeping.md)
- [Qubit](qubit.md)
- [Rabi cycle](rabi-cycle.md)
- [Ramsey interferometry](ramsey-interferometry.md)
- [Schrödinger equation](schrodinger-equation.md)
- [Sequential Bayesian photon counting](sequential-bayesian-photon-counting.md)
- [Single-photon state](single-photon-state.md)
- [Slater determinant](slater-determinant.md)
- [Three-qubit bit-flip syndrome table](three-qubit-bit-flip-syndrome-table.md)
- [Time-independent Schrödinger equation](time-independent-schrodinger-equation.md)
- [Trapped-ion quantum control](trapped-ion-quantum-control.md)
- [Two-channel scattering with flux normalization](two-channel-scattering-with-flux-normalization.md)
- [Two-flavour vacuum survival model](two-flavour-vacuum-survival-model.md)
- [Wave function](wave-function-split.md)
- [Wavefunction normalization](wavefunction-normalization.md)
- [Zero-temperature filling of finite fermion levels](zero-temperature-filling-of-finite-fermion-levels.md)
