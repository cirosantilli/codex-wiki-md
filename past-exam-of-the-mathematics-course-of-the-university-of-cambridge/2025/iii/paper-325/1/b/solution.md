<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the apparatus begin in a ready state $|A_0\rangle$. An ideal unitary measurement interaction is defined on the relevant subspace by

$$
U(|e_i\rangle|A_0\rangle)=|e_i\rangle|i\rangle.
$$

Thus an initial $|\phi\rangle=\sum_i a_i|e_i\rangle$ evolves to the entangled state

$$
|\Psi\rangle=\sum_i a_i|e_i\rangle|i\rangle,
$$

and orthogonality of the pointer states gives

$$
\boxed{\rho_S=\operatorname{Tr}_A|\Psi\rangle\langle\Psi|
=\sum_i|a_i|^2|e_i\rangle\langle e_i|}.
$$

Before the interaction, the [Born rule](../../../../../../born-rule.md) gives

$$
\boxed{\Pr(P_{ij}=1)
=|\langle\psi_{ij}|\phi\rangle|^2
=\frac12|a_i+a_j|^2}.
$$

Afterward,

$$
\boxed{\Pr(P_{ij}=1)
=\operatorname{Tr}(P_{ij}\rho_S)
=\frac12(|a_i|^2+|a_j|^2)}.
$$

The missing cross term is the lost interference between the $i$ and $j$ branches. Entanglement with orthogonal pointer records therefore explains [quantum decoherence](../../../../../../quantum-decoherence.md) and the appearance of a classical mixture to the subsystem. It does not solve the [quantum measurement problem](../../../../../../measurement-problem.md): unitary evolution alone does not explain why one definite pointer value is observed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
