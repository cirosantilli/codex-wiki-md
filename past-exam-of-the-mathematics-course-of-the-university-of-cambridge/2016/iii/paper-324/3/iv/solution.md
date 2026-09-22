<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use [GHZ preparation with Hadamard and controlled-Z gates](../../../../../../ghz-preparation-with-hadamard-and-controlled-z-gates.md) for $n\geq2$. Apply a [Hadamard gate](../../../../../../hadamard-gate.md) to the first [qubit](../../../../../../qubit.md), then a [controlled-NOT gate](../../../../../../controlled-not-gate.md) from that [qubit](../../../../../../qubit.md) to each of the other $n-1$ [qubits](../../../../../../qubit.md). Every controlled-NOT can be written in the allowed gate set as

$$
\operatorname{CNOT}_{1\to j}=H_j\,CZ_{1j}\,H_j.
$$

Indeed conjugating the target $Z$ by $H$ makes the controlled phase into a controlled $X$. The rightmost gate acts first. Consequently the [Clifford circuit](../../../../../../clifford-circuit.md) uses $1+3(n-1)$ allowed gates and gives

$$
\boxed{|\psi\rangle=\frac{|0\rangle^{\otimes n}+|1\rangle^{\otimes n}}{\sqrt2}.}
$$

For every chosen [qubit](../../../../../../qubit.md) $j$, tracing out the other [qubits](../../../../../../qubit.md) yields $\rho_j=\tfrac12(|0\rangle\langle0|+|1\rangle\langle1|)=I/2$. Equivalently, across that [qubit](../../../../../../qubit.md) versus the rest, the displayed state is a [Schmidt decomposition](../../../../../../schmidt-decomposition.md) with two nonzero coefficients $1/\sqrt2$. It is therefore [entangled](../../../../../../entangled-state.md) across every such bipartition.

**[Entanglement](../../../../../../entangled-state.md) does not prevent the polynomial single-output simulation from part (iii).** The simulation follows the measured observable rather than claiming that the intermediate states remain [product states](../../../../../../product-state.md). When $n=1$, there is no remaining subsystem and the requested [entanglement](../../../../../../entangled-state.md) is impossible; the construction and claim require $n\geq2$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
