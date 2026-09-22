<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

An [AND gate](../../../../and-gate.md) maps four possible pairs to one bit and loses information, so it is not reversible. A reversible embedding retains both inputs and uses a target bit:

$$
\boxed{(a,b,c)\longmapsto(a,b,c\oplus ab).}
$$

This is the [Toffoli gate](../../../../toffoli-gate.md); initializing $c=0$ computes $ab$ while preserving enough information to invert the operation.

Classical reversible gates on one or two bits alone cannot synthesize every such operation. Every permutation of two bits is an invertible affine map over the [finite field](../../../../finite-field.md) $\mathbb F_2$: there are $4\cdot|\mathrm{GL}(2,2)|=4\cdot6=24$ of them, exactly the $4!$ permutations. Their extensions to a larger register and their compositions remain affine. The nonlinear term $ab$ in the [Toffoli gate](../../../../toffoli-gate.md) therefore cannot be generated. Three-bit reversible gates remove this obstruction, with ancillary bits initialized appropriately.

There is no conflict with quantum universality: one- and two-[qubit](../../../../qubit.md) gates may pass through [quantum superpositions](../../../../quantum-superposition.md) and use relative [phases](../../../../phase-waves.md) at intermediate steps. They are not restricted to permutations of computational [basis](../../../../basis.md) states at every step. For example the [Hadamard gate](../../../../hadamard-gate.md), [T gate](../../../../t-gate.md) and [CNOT gate](../../../../controlled-not-gate.md) can decompose a [Toffoli gate](../../../../toffoli-gate.md) exactly. Thus the classical affine obstruction does not apply to their intermediate [unitary operators](../../../../unitary-operator.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
