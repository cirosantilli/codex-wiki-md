<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Control all three CNOTs of the [SWAP gate](../../../../swap-gate.md) decomposition by [qubit](../../../../qubit.md) 1. This gives, in temporal order,

$$
T_{1,2\to3},\qquad T_{1,3\to2},\qquad T_{1,2\to3}.
$$

When the first [qubit](../../../../qubit.md) is 0, all three [Toffoli gates](../../../../toffoli-gate.md) do nothing. When it is 1, the three lower-wire CNOTs implement [SWAP gate](../../../../swap-gate.md). The middle panel of the original diagram shows this controlled network.

Only one [Toffoli gate](../../../../toffoli-gate.md) is actually needed. An equivalent circuit is

$$
\boxed{\operatorname{CNOT}_{3\to2},\qquad T_{1,2\to3},\qquad\operatorname{CNOT}_{3\to2}.}
$$

For input $(c,a,b)$, the first gate forms $a\oplus b$ on wire 2. The second changes wire 3 to $b'=b\oplus c(a\oplus b)$, and the final gate gives wire 2 the value $a'=a\oplus c(a\oplus b)$. For $c=0$ this is $(a,b)$; for $c=1$ it is $(b,a)$. The last panel displays the circuit.

The [Hamming-weight obstruction to Fredkin-only Toffoli synthesis](../../../../hamming-weight-obstruction-to-fredkin-only-toffoli-synthesis.md) means that a network of [Fredkin gates](../../../../fredkin-gate.md) alone cannot implement a [Toffoli gate](../../../../toffoli-gate.md) on the same three wires: each [Fredkin gate](../../../../fredkin-gate.md) preserves [computational-basis](../../../../computational-basis.md) [Hamming weight](../../../../hamming-weight.md), whereas [Toffoli gate](../../../../toffoli-gate.md) maps $110$ to $111$. The same obstruction holds if fixed ancillary bits must be returned unchanged. Conservative classical computation can use extra encoded wires and input-dependent garbage, but that is not an ancilla-free coherent three-qubit [Toffoli gate](../../../../toffoli-gate.md) operation. The resources and output encoding would need to be specified before making a different universality claim.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
