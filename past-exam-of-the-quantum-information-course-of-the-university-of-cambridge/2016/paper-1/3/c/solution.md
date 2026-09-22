<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Quantum error correction](../../../../../quantum-error-correction-split.md) encodes a [logical qubit](../../../../../logical-qubit.md) into a larger [Hilbert space](../../../../../hilbert-space-split.md), diagnoses a specified error family with an [error syndrome](../../../../../error-syndrome.md), and reverses it without learning the protected logical amplitudes. It must preserve arbitrary superpositions, not just distinguish two classical codewords.

The [bit-flip repetition code](../../../../../bit-flip-repetition-code.md) encodes

$$
\alpha|0\rangle+\beta|1\rangle\longmapsto\alpha|000\rangle+\beta|111\rangle.
$$

Measure the commuting [stabilizer generators](../../../../../stabilizer-generator.md) $Z_1Z_2$ and $Z_2Z_3$ using ancillary qubits. Their outcomes reveal the parity relations, with the [three-qubit bit-flip syndrome table](../../../../../three-qubit-bit-flip-syndrome-table.md)

$$
\boxed{\begin{array}{c|c|c}
\text{error}&(Z_1Z_2,Z_2Z_3)&\text{recovery}\\\hline
I&(+1,+1)&I\\
X_1&(-1,+1)&X_1\\
X_2&(-1,-1)&X_2\\
X_3&(+1,-1)&X_3
\end{array}}
$$

Both codewords have the same parity checks, so the syndrome does not reveal $\alpha$ or $\beta$. For example, the $X_2$ error produces $\alpha|010\rangle+\beta|101\rangle$; applying $X_2$ restores the encoded superposition. A coherent combination of correctable errors is also recoverable after the syndrome is recorded in an ancilla, by linearity.

This three-qubit code corrects one bit flip, not every one-qubit error. A physical $Z_1$ changes the relative logical phase without a nontrivial bit-flip syndrome. General single-qubit noise is a linear combination of $I,X,Y,Z$; protecting arbitrary single-qubit errors therefore needs a code such as the [Shor code](../../../../../shor-code.md), the [Steane code](../../../../../steane-code.md) or the [five-qubit code](../../../../../five-qubit-error-correcting-code.md), with the corresponding enlarged syndrome structure.

The general exact-recovery criterion is the [Knill--Laflamme condition](../../../../../knill-laflamme-condition.md). For code projector $P$ and error operators $E_r$, there must be constants $C_{rs}$ such that

$$
\boxed{PE_r^\dagger E_sP=C_{rs}P\quad\text{for every }r,s.}
$$

It expresses that the syndrome information can depend on the error but not on the logical state. Encoding entangles several physical qubits; it does not create independent copies of an unknown input, so it respects the [no-cloning theorem](../../../../../no-cloning-theorem.md). Fault-tolerant implementations must also prevent noisy syndrome extraction and recovery gates from spreading an initially correctable error into an uncorrectable one.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
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
