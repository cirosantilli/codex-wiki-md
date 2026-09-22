<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the promised phase as $\phi=2\pi m/8$. Prepare three logical [qubits](../../../../../../qubit.md) in $|+\rangle$ and attach zero ancillas in three blocks of sizes four, two and one. A block of size $r$ is prepared by fanout [CNOT gates](../../../../../../controlled-not-gate.md) as

$$
\frac{|0^r\rangle+|1^r\rangle}{\sqrt2}.
$$

Apply one copy of $U_\phi$ to every physical [qubit](../../../../../../qubit.md) in every block, all in the same time step. Undo each fanout. The logical block output is $(|0\rangle+e^{ir\phi}|1\rangle)/\sqrt2$ and every ancillary wire returns to zero. This is [parallel phase multiplication by coherent fanout](../../../../../../parallel-phase-multiplication-by-coherent-fanout.md); its intermediate [entanglement](../../../../../../entangled-state.md) copies basis labels, and does not clone an arbitrary [quantum state](../../../../../../quantum-state.md).

For block weights $4,2,1$, the three logical wires now contain

$$
\bigotimes_{r\in(4,2,1)}\frac{|0\rangle+e^{ir\phi}|1\rangle}{\sqrt2}
=\frac1{\sqrt8}\sum_{l=0}^7e^{i\phi l}|l\rangle.
$$

Apply the specified negative-sign [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) and measure. Part (a) gives label $m$ deterministically. Thus **seven parallel phase-gate applications, on three logical wires and four ancillas, identify the phase in one oracle time step**. Preparation, uncomputation and the Fourier transform cost no time under the stated model; using serial powers would not meet the time requirement.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
