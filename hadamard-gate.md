# Hadamard gate

↑ **Parent:** [Hadamard transform](hadamard-transform.md)

The [Hadamard gate](hadamard-gate.md) is the [unitary operator](unitary-operator.md)

$$
H=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad H^2=I,
$$

where $I$ is the [identity operator](identity-operator.md). It maps the [computational basis](computational-basis.md) to the [Hadamard basis](hadamard-basis.md):

$$
|0\rangle\mapsto\frac{|0\rangle+|1\rangle}{\sqrt2},
\qquad
|1\rangle\mapsto\frac{|0\rangle-|1\rangle}{\sqrt2}.
$$

These outputs have equal [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) probabilities, but their relative [quantum phase](quantum-phase.md) differs. Applying another [Hadamard gate](hadamard-gate.md) sends them to different definite outputs. Calling this gate a classical coin toss would discard precisely the information that makes this possible. [Watrous, IBM Quantum Learning, unitary operations on qubits](https://quantum.cloud.ibm.com/learning/en/courses/basics-of-quantum-information/single-systems/quantum-information).

Starting from $|0\rangle$, compare two [quantum circuits](quantum-circuit-split.md), reading matrix products from right to left:

$$
HH|0\rangle=|0\rangle,\qquad HZH|0\rangle=|1\rangle.
$$

Here $Z$ is the [Pauli Z gate](pauli-z-gate.md). After the first [Hadamard gate](hadamard-gate.md), the [probability amplitudes](probability-amplitude.md) are $(1/\sqrt2,1/\sqrt2)$. Inserting $Z$ changes them to $(1/\sqrt2,-1/\sqrt2)$ without changing their squared magnitudes. At the final gate, the contributions to output zero cancel and those to output one add. Without $Z$, cancellation occurs at output one instead. This is controlled [interference](interference-wave-propagation.md), with the [quantum phase](quantum-phase.md) determining which answer emerges.

The same calculation works for any [phase gate](phase-gate.md) $P_\phi=\operatorname{diag}(1,e^{i\phi})$:

$$
HP_\phi H|0\rangle=\frac{1+e^{i\phi}}2|0\rangle+\frac{1-e^{i\phi}}2|1\rangle,
\qquad P(1)=\sin^2(\phi/2),\quad P(0)=\cos^2(\phi/2).
$$

For example, $\phi=\pi/3$ gives $P(1)=1/4$, while $\phi=\pi/2$ gives $P(1)=1/2$. The output-one amplitude at $\phi=\pi/2$ is $(1-i)/2$: its two complex contributions add before the [Born rule](born-rule.md) is applied. A [phase gate](phase-gate.md) alone leaves the populations unchanged; recombination converts its relative [quantum phase](quantum-phase.md) into observable [probabilities](probability.md).

<a id="image-hadamard-interference-a-relative-phase-changes-output-probabilities-through-complex-amplitude-addition-the-dotted-circle-traces-the-output-one-amplitude-as-the-phase-varies"></a>
![](hadamard-interference.png)

**[Figure 1](#image-hadamard-interference-a-relative-phase-changes-output-probabilities-through-complex-amplitude-addition-the-dotted-circle-traces-the-output-one-amplitude-as-the-phase-varies). Hadamard interference: a relative phase changes output probabilities through complex amplitude addition; the dotted circle traces the output-one amplitude as the phase varies**.

If [quantum decoherence](quantum-decoherence.md) completely removes the [computational basis](computational-basis.md) coherence between the gates, the intermediate [density matrix](density-matrix-split.md) becomes $I/2$. Both the [phase gate](phase-gate.md) and final [Hadamard gate](hadamard-gate.md) leave $I/2$ unchanged, so $P(1)=1/2$ for every $\phi$. The disappearing fringe explains why preserving [quantum coherence](quantum-coherence-in-a-specified-basis.md) matters: it enables the gate sequence to carry phase information into the final measurement.

**Table of contents**

- [Hadamard-phase-Hadamard qubit rotation](hadamard-phase-hadamard-qubit-rotation.md)
- [Photon-number reference for a Hadamard gate](photon-number-reference-for-a-hadamard-gate.md)
- [Uniform quantum superposition](uniform-quantum-superposition.md)

## ↑ Ancestors (5)

1. [Hadamard transform](hadamard-transform.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (103)

- [Backward Pauli updates for Hadamard and phase gates](backward-pauli-updates-for-hadamard-and-phase-gates.md)
- [Bell-basis conversion circuit](bell-basis-conversion-circuit.md)
- [Born rule](born-rule.md)
- [Controlled-Z gate](controlled-z-gate.md)
- [Deutsch algorithm](deutsch-algorithm.md)
- [Deutsch algorithm with pure dephasing](deutsch-algorithm-with-pure-dephasing.md)
- [Dicke-resource telecloning](dicke-resource-telecloning.md)
- [Dyadic quantum Fourier transform circuit](dyadic-quantum-fourier-transform-circuit.md)
- [Entanglement-assisted nondemolition parity measurement](entanglement-assisted-nondemolition-parity-measurement.md)
- [GHZ preparation with Hadamard and controlled-Z gates](ghz-preparation-with-hadamard-and-controlled-z-gates.md)
- [Hadamard gate](hadamard-gate.md)
- [Hadamard-phase-Hadamard qubit rotation](hadamard-phase-hadamard-qubit-rotation.md)
- [Hadamard transform](hadamard-transform.md)
- [Inverse quantum circuit](inverse-quantum-circuit.md)
- [J gate in measurement-based quantum computation](j-gate-in-measurement-based-quantum-computation.md)
- [J-gate phase-error operator norm](j-gate-phase-error-operator-norm.md)
- [Logical Hadamard convention for a phase-flip repetition code](logical-hadamard-convention-for-a-phase-flip-repetition-code.md)
- [Mixed-state Hadamard-test quadratures](mixed-state-hadamard-test-quadratures.md)
- [Nonadaptive Hadamard–CNOT measurement pattern](nonadaptive-hadamard-cnot-measurement-pattern.md)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/3/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-60/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/4/b/protocol-1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/4/b/protocol-2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57/3/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/15d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/3/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/4/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/10c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/15c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/15c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/15c/d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/15c/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/10d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/10d/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/15d/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-324/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-324/4/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/10c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-324/3/a/ii/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2012/paper-1/3/c/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2015/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2016/paper-1/3/b/solution.md)
- [Phase-flip protection by Hadamard conjugation](phase-flip-protection-by-hadamard-conjugation.md)
- [Premature basis announcement in quantum key distribution](premature-basis-announcement-in-quantum-key-distribution.md)
- [Quantum logic gate](quantum-logic-gate.md)
- [Quantum superposition](quantum-superposition.md)
- [Quantum theory](quantum-theory-split.md)
- [Single-qubit interference with conditional environment states](single-qubit-interference-with-conditional-environment-states.md)
- [Uniform superposition state](uniform-superposition-state.md)
