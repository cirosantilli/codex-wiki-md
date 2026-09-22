<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a Hermitian [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md), $[\sigma_m,\sigma_n]^\dagger=-[\sigma_m,\sigma_n]$. Consequently

$$
L_{mn}^*=-i\operatorname{Tr}([\sigma_m,\sigma_n]^\dagger H)
=i\operatorname{Tr}(H[\sigma_m,\sigma_n])=L_{mn}.
$$

Swapping $m,n$ changes the sign of the [commutator](../../../../../../commutator.md), so $L_{nm}=-L_{mn}$. The generator is therefore real and antisymmetric. Its last column vanishes because the identity commutes with $H$, so $c=0$ and the traceless block satisfies $A^T=-A$.

For constant $H$, the [Bloch vector](../../../../../../bloch-vector.md) evolves by $s(t)=R(t)s(0)$ with $R(t)=e^{At}$. Direct differentiation gives

$$
\frac d{dt}(R^TR)=R^T(A^T+A)R=0,
\qquad R(0)=I.
$$

Hence $R^TR=I$. Its [determinant](../../../../../../determinant.md) is continuously connected to one and cannot change between the two possible values $\pm1$, so $\det R=1$. This proves that the evolution is a rotation in the [special orthogonal group](../../../../../../special-orthogonal-group.md). A time-dependent Hermitian [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) has the same conclusion from $\dot R=A(t)R$.

These [Hamiltonian rotations of Bloch vectors](../../../../../../hamiltonian-rotations-of-bloch-vectors.md) preserve the Euclidean norm and [purity of a density operator](../../../../../../purity-of-a-density-operator.md). For $N>2$, not every rotation of the ambient sphere is a physical unitary conjugation: the higher-dimensional positivity constraints and full [spectrum](../../../../../../spectrum-functional-analysis.md) of the [density operator](../../../../../../density-matrix.md) impose further restrictions.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
