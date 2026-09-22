<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For second-[qubit](../../../../qubit.md) inputs $|0\rangle$ and $|1\rangle$, [c](../c.md) gives control [expectation values](../../../../expectation-value.md) $\operatorname{Re}U_{00}$ and $\operatorname{Re}U_{11}$. Preparing the [maximally mixed state](../../../../maximally-mixed-state.md) $I/2$ is equivalent to choosing these inputs independently with equal [probability](../../../../probability.md) and discarding the choice. Linearity of the [density operator](../../../../density-matrix-split.md) evolution and [quantum measurement](../../../../quantum-measurement-split.md) probabilities therefore gives

$$
\langle Z\rangle_{I/2}
=\tfrac12\operatorname{Re}U_{00}+\tfrac12\operatorname{Re}U_{11}
=\tfrac12\operatorname{Re}\operatorname{Tr}U.
$$

Hence

$$
\boxed{\operatorname{Re}\operatorname{Tr}U=2(P_0-P_1).}
$$

The factor two is essential: the [Hadamard test](../../../../hadamard-test.md) directly estimates the normalized [trace](../../../../matrix-trace.md). More generally, a target [density operator](../../../../density-matrix-split.md) $\rho$ gives $\langle Z\rangle=\operatorname{Re}\operatorname{Tr}(\rho U)$. This argument never requires knowledge of the [eigenvectors](../../../../eigenvector.md) of $U$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
