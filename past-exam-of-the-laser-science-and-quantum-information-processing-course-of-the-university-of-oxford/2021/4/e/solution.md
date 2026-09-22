<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A bipartite [pure state](../../../../pure-state.md) is entangled when it cannot be written $|\alpha\rangle_a\otimes|\beta\rangle_b$. For [mixed states](../../../../mixed-state.md), the corresponding definition excludes every convex mixture of [product states](../../../../product-state.md), not just a single [product state](../../../../product-state.md).

Apply a [Hadamard gate](../../../../hadamard-gate.md) to ion $a$, followed by the [CNOT gate](../../../../controlled-not-gate.md) of part (d):

$$
|gg\rangle\xrightarrow{H_a}\frac{|gg\rangle+|eg\rangle}{\sqrt2}
\xrightarrow{C_X}\boxed{\frac{|gg\rangle+|ee\rangle}{\sqrt2}.}
$$

The lower network in the figure shows this [Bell pair](../../../../bell-pair.md) preparation. Either ion alone has [reduced density matrix](../../../../reduced-density-matrix.md) $I/2$, whereas the joint [quantum state](../../../../quantum-state.md) is pure; hence the joint [quantum state](../../../../quantum-state.md) cannot be a [product state](../../../../product-state.md). The entangling operation can be expanded into $H_b,G,Z_a,H_b$ exactly as above.

## ↑ Ancestors (12)

1. [E](../e.md)
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
