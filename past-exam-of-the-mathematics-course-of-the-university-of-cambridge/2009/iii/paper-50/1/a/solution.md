<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the code, and let $\{E_a\}$ be the specified error operators, including their [linear span](../../../../../../linear-span.md). The necessary and sufficient [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) is

$$
\boxed{PE_a^\dagger E_bP=C_{ab}P\quad\text{for every }a,b,}
$$

where the scalar [matrix](../../../../../../matrix.md) $C$ is independent of the encoded state. In an [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|j_L\rangle\}$ of the code this means

$$
\langle i_L|E_a^\dagger E_b|j_L\rangle=C_{ab}\delta_{ij}.
$$

There must be one recovery [quantum channel](../../../../../../quantum-channel.md) which corrects every allowed error channel, rather than a different recovery chosen using the unknown logical input.

The scalar condition means that any information carried away by the errors depends on their labels but not on the encoded amplitudes. To see how recovery works, diagonalize the [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) $C$ and take corresponding linear combinations $F_\ell$ of the errors. Then $PF_\ell^\dagger F_mP=\lambda_\ell\delta_{\ell m}P$. For each positive $\lambda_\ell$, the map $F_\ell P/\sqrt{\lambda_\ell}$ is an [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) into an error-image subspace, and these subspaces are mutually orthogonal. Measuring their label and reversing the associated [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md) recovers the logical state without measuring its amplitudes. Zero [eigenvalues](../../../../../../eigenvalue.md) correspond to errors that annihilate the code. This also explains why the condition corrects arbitrary coherent combinations of the listed errors.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
