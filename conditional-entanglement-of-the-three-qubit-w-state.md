# Conditional entanglement of the three-qubit W state

↑ **Parent:** [W state](w-state.md)

Every rank-one [projective measurement](projective-measurement.md) of one [qubit](qubit.md) of the three-qubit [W state](w-state.md) has at least one nonzero-probability outcome whose other two [qubits](qubit.md) remain entangled. To see this, contract the measured factor against $\langle u|$, where $|u\rangle=a|0\rangle+b|1\rangle$. The unnormalized [tensor-product coefficient matrix](tensor-product-coefficient-matrix.md) of the other pair is

$$
C_u=\frac1{\sqrt3}\begin{pmatrix}\overline b&\overline a\\\overline a&0\end{pmatrix},\qquad\det C_u=-\frac{\overline a^{\,2}}3.
$$

At least one [vector](vector.md) in a complete measurement basis has $a\ne0$, giving nonzero determinant and an entangled conditional branch. Its [probability](probability.md) $(2|a|^2+|b|^2)/3$ is positive. This property survives local unitary changes of basis. The [GHZ state](greenberger-horne-zeilinger-state.md) lacks it because [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) of one [qubit](qubit.md) leaves a [product state](product-state.md) on each branch, so the property also separates the states under [local-unitary equivalence](local-unitary-equivalence.md).

## ↑ Ancestors (8)

1. [W state](w-state.md)
2. [Dicke state](dicke-state.md)
3. [Quantum state](quantum-state.md)
4. [Quantum system](quantum-system-split.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/quantum-information/2/d/i/solution.md)
