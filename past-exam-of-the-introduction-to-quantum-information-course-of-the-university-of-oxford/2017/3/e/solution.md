<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The input is the [Bell state](../../../../bell-state-split.md) $\rho=|\Phi^+\rangle\langle\Phi^+|$, where $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$. Acting on the first [qubit](../../../../qubit.md) reverses the signs of all three terms containing its [Pauli matrices](../../../../pauli-matrices.md), so in [computational basis](../../../../computational-basis.md) order $00,01,10,11$ the output is

$$
\boxed{(\mathcal N\otimes\operatorname{id})(\rho)
=\frac14(I\otimes I-X\otimes X+Y\otimes Y-Z\otimes Z)
=\begin{pmatrix}
0&0&0&-1/2\\
0&1/2&0&0\\
0&0&1/2&0\\
-1/2&0&0&0
\end{pmatrix}.}
$$

Its [eigenvalues](../../../../eigenvalue.md) are $\boxed{-1/2,1/2,1/2,1/2}$: in particular, its [expectation value](../../../../expectation-value.md) in $|\Phi^+\rangle$ is $-1/2$. It therefore fails to be [positive semidefinite](../../../../positive-semidefinite-matrix.md), although its [trace](../../../../matrix-trace.md) remains one. This single [entangled state](../../../../entangled-state.md) proves that the [universal NOT gate](../../../../universal-not-gate.md) is **positive but not completely positive**, so it cannot be a deterministic physical [quantum channel](../../../../quantum-channel.md) on an arbitrary input.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
