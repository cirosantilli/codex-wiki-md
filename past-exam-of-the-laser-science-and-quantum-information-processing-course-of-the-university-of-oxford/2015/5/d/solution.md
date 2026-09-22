<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$ be the [Pauli X eigenstates](../../../../pauli-x-eigenstate.md). Encode

$$
\boxed{|0_L\rangle=|+ -\rangle,\qquad |1_L\rangle=|- +\rangle.}
$$

Both have zero total $X$ eigenvalue, so $R_x(\phi)\otimes R_x(\phi)$ is the identity on their span. This is the [decoherence-free subspace](../../../../decoherence-free-subspace.md) obtained from the previous code by applying a [Hadamard gate](../../../../hadamard-gate.md) to each physical [qubit](../../../../qubit.md).

Since $Z|+\rangle=|-\rangle$ and $Z|-\rangle=|+\rangle$, a correlated $Z\otimes Z$ error exchanges the codewords. It acts as logical $X_L$, not as harmless identity. The [Pauli Y gate](../../../../pauli-y-gate.md) obeys $Y|+\rangle=-i|-\rangle$ and $Y|-\rangle=i|+\rangle$, so

$$
\boxed{(Z\otimes Z)|\psi_L\rangle=(Y\otimes Y)|\psi_L\rangle=X_L|\psi_L\rangle.}
$$

The phases cancel within each codeword. Thus either unknown correlated gate gives a logical bit error on a general encoded state, though a logical $X_L$ [eigenstate](../../../../eigenstate.md) is unchanged as a physical ray. The code prevents collective $x$ rotations, not every possible correlated error.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
