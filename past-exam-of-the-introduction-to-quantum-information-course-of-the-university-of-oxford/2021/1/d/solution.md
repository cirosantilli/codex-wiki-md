<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Direct [matrix multiplication](../../../../matrix-multiplication.md) gives

$$
\begin{array}{c|ccc}
 &X&Y&Z\\\hline
HPH^\dagger&Z&-Y&X\\
SPS^\dagger&Y&-X&Z.
\end{array}
$$

Thus each generating [Clifford gate](../../../../clifford-gate.md) conjugates every [Pauli operator](../../../../pauli-operator.md) to another Pauli operator up to sign. Repeated conjugation proves the same for every product of generators and their inverses, hence for the [Clifford group](../../../../clifford-group-quantum-computing.md). For Hermitian Pauli observables the possible phases here are signs; arbitrary Pauli-group elements also include their conventional phases.

If $P|\psi\rangle=\lambda|\psi\rangle$, then $(CPC^\dagger)C|\psi\rangle=\lambda C|\psi\rangle$. Therefore $C|\psi\rangle$ is another [Pauli eigenstate](../../../../pauli-eigenstate.md). Every single-qubit Clifford circuit consequently permutes the six Pauli vertices of the [stabilizer octahedron](../../../../stabilizer-octahedron.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
