<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The filtered decomposition is not necessarily frustration-free.** Commuting with $P_0$ makes $|\phi_0\rangle$ an [eigenvector](../../../../../../eigenvector.md) of each term; it does not make that [eigenvector](../../../../../../eigenvector.md) a lowest-energy state of each term. This is the distinction expressed by [commuting with a ground projector does not imply frustration freeness](../../../../../../commuting-with-a-ground-projector-does-not-imply-frustration-freeness.md).

For an explicit positive, two-local counterexample on three [qubits](../../../../../../qubit.md), let $P_0^{(i)}=|0\rangle\langle0|_i$ and $P_1^{(i)}=|1\rangle\langle1|_i$, and use the two distinct interaction sets $\{1,2\}$ and $\{2,3\}$:

$$
h_{12}=P_1^{(1)}+P_0^{(2)},\qquad
h_{23}=P_1^{(3)}+2P_1^{(2)}.
$$

Both are [positive semidefinite](../../../../../../positive-semidefinite-matrix.md) and commute with their sum. The total energy on a computational basis vector is

$$
E(b_1,b_2,b_3)=b_1+b_3+1+b_2.
$$

Thus $H=h_{12}+h_{23}$ has unique [ground state](../../../../../../ground-state.md) $|000\rangle$, energy $1$, and [spectral gap](../../../../../../spectral-gap.md) $1$. Since $[H,h_{12}]=[H,h_{23}]=0$, [spectral filtering of Hamiltonian terms](../../../../../../spectral-filtering-of-hamiltonian-terms.md) leaves both terms unchanged for every normalized filter:

$$
g^{(12)}=h_{12},\qquad g^{(23)}=h_{23}.
$$

But $h_{12}|000\rangle=|000\rangle$, whereas $h_{12}|010\rangle=0$. The global [ground state](../../../../../../ground-state.md) therefore does not minimize $g^{(12)}$, proving that the resulting decomposition is not a [frustration-free Hamiltonian](../../../../../../frustration-free-quantum-hamiltonian.md).

There is a useful positive result if the original decomposition already is a [frustration-free Hamiltonian](../../../../../../frustration-free-quantum-hamiltonian.md). If $a_Z=\lambda_{\min}(h_Z)$ and $h_Z|\phi_0\rangle=a_Z|\phi_0\rangle$, then $h_Z-a_ZI\geq0$. Averaging its unitary conjugates with nonnegative $w$ gives $g^{(Z)}-a_ZI\geq0$, while $g^{(Z)}|\phi_0\rangle=a_Z|\phi_0\rangle$. Thus [filtering preserves existing frustration freeness](../../../../../../filtering-preserves-existing-frustration-freeness.md); it does not create it for an arbitrary gapped Hamiltonian.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
