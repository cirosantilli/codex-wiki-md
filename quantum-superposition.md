# Quantum superposition

↑ **Parent:** [Quantum state](quantum-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_superposition)

A quantum superposition is a [linear combination](linear-combination.md) of [quantum state](quantum-state.md) vectors in a complex [Hilbert space](hilbert-space-split.md). In a specified [orthonormal basis](orthonormal-basis.md), a normalized [pure state](pure-state.md) has the displayed expansion, where $a_j$ are [probability amplitudes](probability-amplitude.md). A nonzero [linear combination](linear-combination.md) can always be normalized; an arbitrary sum of normalized vectors need not already have [norm](norm.md) one. Having more than one nonzero component depends on the chosen [basis](basis.md): the [Hadamard basis](hadamard-basis.md) vector $|+\rangle$ is a [quantum superposition](quantum-superposition.md) of the two [computational-basis states](computational-basis-state.md), but is a single vector of the [Hadamard basis](hadamard-basis.md). [Zwiebach, MIT 8.04, lecture 1, section 4, pp. 10–12](https://ocw.mit.edu/courses/8-04-quantum-physics-i-spring-2016/7f930e013cef9cd7dec5aa88baa83f0a_MIT8_04S16_LecNotes1.pdf).

The distinction from classical ignorance is quantitative. Consider the normalized [qubit](qubit.md) [quantum state](quantum-state.md)

$$
|\psi_\phi\rangle=\frac{\sqrt3}{2}|0\rangle+\frac{e^{i\phi}}2|1\rangle.
$$

Its [density operator](density-matrix.md), written in the [computational basis](computational-basis.md), is

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

The [density matrix](density-matrix.md) representation retains this distinction between a [pure state](pure-state.md) and a [mixed state](mixed-state.md). [Watrous, IBM Quantum Learning, Density matrix basics, Interpretation of density matrices and Connection to quantum state vectors](https://quantum.cloud.ibm.com/learning/en/courses/general-formulation-of-quantum-information/density-matrices/density-matrix-basics).

For example, at $\phi=0$, the [quantum superposition](quantum-superposition.md) yields the plus outcome with [probability](probability.md) about $0.9330$, whereas the [mixed state](mixed-state.md) yields it with [probability](probability.md) $0.5$. At $\phi=\pi/2$ these particular [probabilities](probability.md) agree, although the [density matrices](density-matrix.md) still differ: equality for one measurement does not establish equality of [quantum states](quantum-state.md). The [probability amplitude](probability-amplitude.md) figure shows the comparison throughout a full cycle of relative [quantum phase](quantum-phase.md).

This is why a [quantum superposition](quantum-superposition.md) is useful: [quantum gates](quantum-logic-gate.md) act linearly on its [probability amplitudes](probability-amplitude.md), and [unitary operators](unitary-operator.md) preserve the full [pure state](pure-state.md) information, including relative [quantum phases](quantum-phase.md). A [Hadamard gate](hadamard-gate.md) can turn otherwise hidden [quantum coherence](quantum-coherence-in-a-specified-basis.md) into different outcome [probabilities](probability.md). The beautiful feature is that the same basis weights can support different predictions when amplitudes recombine. The expansion specifies a preparation and its measurement predictions; it does not assign every unmeasured outcome a simultaneous classical value. See [projective measurement](projective-measurement.md) for the separate question of the conditional state after a measurement.

## ↑ Ancestors (6)

1. [Quantum state](quantum-state.md)
2. [Quantum system](quantum-system.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (25)

- [Amplitude amplification](amplitude-amplification.md)
- [Born rule](born-rule.md)
- [Elitzur-Vaidman bomb tester](elitzur-vaidman-bomb-tester.md)
- [Energy eigenspace](energy-eigenspace.md)
- [Energy eigenstate](energy-eigenstate.md)
- [Excited state](excited-state.md)
- [Exclusion versus particle position](exclusion-versus-particle-position.md)
- [Ground-state degeneracy](ground-state-degeneracy.md)
- [Infinite square well](infinite-square-well.md)
- [Mixed state](mixed-state.md)
- [Nondegenerate phase-flip correction in the Steane code](nondegenerate-phase-flip-correction-in-the-steane-code.md)
- [Parity computation by CNOT gates](parity-computation-by-cnot-gates.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/a/solution.md)
- [Probability amplitude](probability-amplitude.md)
- [Quantum error correction](quantum-error-correction-split.md)
- [Quantum mechanics](quantum-mechanics-split.md)
- [Quantum superposition](quantum-superposition.md)
- [Qubit](qubit.md)
- [Slater determinant](slater-determinant.md)
- [Three-qubit bit-flip syndrome table](three-qubit-bit-flip-syndrome-table.md)
- [Wave function](wave-function.md)
- [Wavefunction normalization](wavefunction-normalization.md)
- [Zero-temperature filling of finite fermion levels](zero-temperature-filling-of-finite-fermion-levels.md)
