<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $|\psi\rangle=a|0\rangle+b|1\rangle$ and $|\phi\rangle=c|0\rangle+d|1\rangle$ be normalized [qubit states](../../../../qubit-state.md). By [linearity](../../../../linearity.md), the [SWAP gate](../../../../swap-gate.md) gives

$$
\begin{aligned}
\mathrm{SWAP}(|\psi\rangle\otimes|\phi\rangle)
&=ac|00\rangle+ad|10\rangle+bc|01\rangle+bd|11\rangle\\
&=(c|0\rangle+d|1\rangle)\otimes(a|0\rangle+b|1\rangle)\\
&=\boxed{|\phi\rangle\otimes|\psi\rangle.}
\end{aligned}
$$

The output remains a [product state](../../../../product-state.md). Single-[qubit](../../../../qubit.md) [unitary operators](../../../../unitary-operator.md) also preserve [product states](../../../../product-state.md), so an induction over any [quantum circuit](../../../../quantum-circuit-split.md) made from these operations shows that it cannot create [quantum entanglement](../../../../entangled-state.md) from a [product state](../../../../product-state.md). Equivalently, $\mathrm{SWAP}(A\otimes B)=(B\otimes A)\mathrm{SWAP}$ moves every exchange through the local operations, leaving only local gates and a permutation of wires. This is the [product-state obstruction to SWAP universality](../../../../product-state-obstruction-to-swap-universality.md).

Consequently **[SWAP gates](../../../../swap-gate.md) and arbitrary single-[qubit](../../../../qubit.md) gates do not form a [universal quantum gate set](../../../../universal-quantum-gate-set.md)**. For example, they cannot map $|00\rangle$ to the [Bell state](../../../../bell-state-split.md) $(|00\rangle+|11\rangle)/\sqrt2$, whereas a [Hadamard gate](../../../../hadamard-gate.md) followed by a [CNOT gate](../../../../controlled-not-gate.md) does so.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [8](../../8-split.md)
3. [2008](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
