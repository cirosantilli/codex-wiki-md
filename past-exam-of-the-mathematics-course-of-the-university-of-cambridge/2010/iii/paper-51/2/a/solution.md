<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce the orthonormal local vectors $|+\rangle=(|1\rangle+|2\rangle)/\sqrt2$ and $|-\rangle=(|1\rangle-|2\rangle)/\sqrt2$. Reexpressing the second state's factors in this basis gives its [Schmidt decomposition](../../../../../../schmidt-decomposition.md)

$$
|\phi_2\rangle=\frac1{\sqrt3}|+\rangle_A|+\rangle_B+\sqrt{\frac23}|-\rangle_A|-\rangle_B.
$$

The squared [Schmidt coefficients](../../../../../../schmidt-coefficient.md) are therefore $1/3,2/3$, whereas those of the first state are $1/2,1/2$.

To see directly why these distinguish the states, a [local unitary operation](../../../../../../local-unitary-operation.md) $U_A\otimes U_B$ changes the [reduced density matrix](../../../../../../reduced-density-matrix.md) to

$$
\rho_A' =\operatorname{Tr}_B[(U_A\otimes U_B)\rho_{AB}(U_A^\dagger\otimes U_B^\dagger)]
=U_A\rho_AU_A^\dagger.
$$

This is [local-unitary invariance of reduced-state spectra](../../../../../../local-unitary-invariance-of-reduced-state-spectra.md): the unitary on the traced subsystem cancels, and conjugation on $A$ leaves its [eigenvalues](../../../../../../eigenvalue.md) unchanged. Here the reductions are

$$
\rho_A^{(1)}=\frac I2,\qquad
\rho_A^{(2)}=\frac13|+\rangle\langle+|+\frac23|-\rangle\langle-|
=\begin{pmatrix}1/2&-1/6\\-1/6&1/2\end{pmatrix}.
$$

Their spectra differ. Hence **no pair of local unitary operations carries the first state to the second**. More generally, normalized bipartite pure states are locally unitarily equivalent exactly when their squared Schmidt coefficients agree, including multiplicities; sufficiency follows by mapping one pair of Schmidt bases to the other.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
