<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [qubit](../../../../../qubit.md) has state $\alpha|0\rangle+\beta|1\rangle$ with $|\alpha|^2+|\beta|^2=1$. An $n$-qubit register occupies a $2^n$-dimensional [Hilbert space](../../../../../hilbert-space-split.md) and may contain entanglement. This large state space does not mean that a measurement reads out all its complex amplitudes: computational-basis outcomes occur with the [Born rule](../../../../../born-rule.md) probabilities.

A [quantum circuit](../../../../../quantum-circuit-split.md) prepares a register, applies [quantum gates](../../../../../quantum-logic-gate.md), and measures selected outputs, possibly using classical feed-forward. Closed gates are [unitary operators](../../../../../unitary-operator.md) and therefore reversible; initialization, measurement and discarding can be treated using a larger system and environment. Single-qubit rotations together with an entangling two-qubit gate give a [universal quantum gate set](../../../../../universal-quantum-gate-set.md). The [CNOT gate](../../../../../controlled-not-gate.md) acts as $|x,y\rangle\mapsto|x,y\oplus x\rangle$.

For example, a [Hadamard gate](../../../../../hadamard-gate.md) on the first qubit of $|00\rangle$ followed by a CNOT creates $(|00\rangle+|11\rangle)/\sqrt2$. A Hadamard produces amplitudes with relative signs, so later gates can make unwanted alternatives interfere destructively and useful alternatives reinforce. [Quantum algorithms](../../../../../quantum-algorithm.md) organize this interference to improve a specified computational task; superposition alone does not supply an arbitrary speedup or permit reading every branch.

A finite discrete universal set such as Clifford gates together with a non-Clifford phase gate approximates general unitaries to chosen precision. Runtime includes the number of gates, repetitions and classical processing. Measurement outcomes may require multiple runs to estimate a probability or amplify success.

[Quantum decoherence](../../../../../quantum-decoherence.md) and imperfect gates limit an implementation. [Quantum error correction](../../../../../quantum-error-correction-split.md) encodes logical information into several physical qubits and measures error syndromes without directly learning the encoded amplitudes. Under appropriate noise and control assumptions, fault tolerance permits reliable longer computations; simply maintaining an isolated ideal state is not a realistic account of a large processor.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the quantum information course of the University of Cambridge](../../../../split.md)
6. [Quantum Information course of the University of Cambridge](../../../../../quantum-information-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
