<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write the [unitary conjugation](../../../../../../unitary-conjugation.md) as $\rho(t)=U(t)\rho(0)U(t)^\dagger$. The identity component is unchanged, and the generalized [Bloch vector](../../../../../../bloch-vector.md) transforms by

$$
s_k(t)=\sum_\ell O_{k\ell}(U(t))s_\ell(0),\qquad O_{k\ell}(U)=\operatorname{Tr}(\sigma_kU\sigma_\ell U^\dagger).
$$

These coefficients are real, by the same trace argument as in part (a). [Unitary conjugation](../../../../../../unitary-conjugation.md) preserves the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md), so the conjugated traceless generators form another [orthonormal basis](../../../../../../orthonormal-basis.md). It follows that $O(U)^TO(U)=I$. The [unitary group](../../../../../../unitary-group.md) is connected, $O(I)=I$, and the [determinant](../../../../../../determinant.md) of an orthogonal [matrix](../../../../../../matrix.md) is $\pm1$; hence $\det O(U)=1$. Thus **Hamiltonian evolution rotates the generalized Bloch vector by an element of $SO(N^2-1)$**.

Equivalently, in units $\hbar=1$, the [Von Neumann equation](../../../../../../von-neumann-equation.md) gives

$$
\dot s_k=\sum_\ell A_{k\ell}s_\ell,\qquad A_{k\ell}=-i\operatorname{Tr}(\sigma_k[H,\sigma_\ell]).
$$

Cyclicity of the [trace](../../../../../../matrix-trace.md) shows $A_{k\ell}=-A_{\ell k}$, so $A$ is a real [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md). This is the generator form of [Hamiltonian rotations of Bloch vectors](../../../../../../hamiltonian-rotations-of-bloch-vectors.md), valid also for a time-dependent [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md). For $N>2$, Hamiltonians generally realize only a proper subgroup of all rotations of this real space; they preserve the whole density-operator [spectrum](../../../../../../spectrum-functional-analysis.md), not merely its [purity of a density operator](../../../../../../purity-of-a-density-operator.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
