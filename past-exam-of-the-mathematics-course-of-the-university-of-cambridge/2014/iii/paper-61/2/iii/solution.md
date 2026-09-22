<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Prepare the two data [qubits](../../../../../../qubit.md) in $|s\rangle=\tfrac12\sum_{x\in B_2}|x\rangle$ and a phase [ancilla qubit](../../../../../../ancilla-qubit.md) in $|{-}\rangle$. A single [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) query flips only the marked amplitude. Its success fraction is $p=1/4$, so $\theta=\pi/6$ in [amplitude amplification](../../../../../../amplitude-amplification.md). The fixed diffusion reflection $D=2|s\rangle\langle s|-I$ gives $\sin(3\theta)=1$ after one iteration.

Directly, after the query the marked amplitude is $-1/2$ and the other three are $1/2$. Their mean is $1/4$. The diffusion reflection replaces each amplitude $c_x$ by $2(1/4)-c_x$, yielding one at the marked input and zero elsewhere. Thus

$$
\boxed{D U_f\bigl(|s\rangle|{-}\rangle\bigr)=|x_*\rangle|{-}\rangle}.
$$

Here $U_f$ is understood with its target [ancilla qubit](../../../../../../ancilla-qubit.md), and $D$ acts only on the data. It is independent of $f$: $D=H^{\otimes2}(2|00\rangle\langle00|-I)H^{\otimes2}$, with the central diagonal gate implementable using two [Pauli Z gates](../../../../../../pauli-z-gate.md) and one [Controlled-Z gate](../../../../../../controlled-z-gate.md). Measuring the data in the [computational basis](../../../../../../computational-basis.md) therefore finds the unique marked string with certainty after one oracle query.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
