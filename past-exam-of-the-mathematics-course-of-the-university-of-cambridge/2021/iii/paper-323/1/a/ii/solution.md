<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a purification $|\Psi_\rho\rangle_{RA}$ of $\rho$, the [entanglement fidelity](../../../../../../../entanglement-fidelity.md) is

$$
F_e(\rho,\Lambda)=
\langle\Psi_\rho|
(\operatorname{id}_R\otimes\Lambda)
(|\Psi_\rho\rangle\langle\Psi_\rho|)
|\Psi_\rho\rangle.
$$

Using a [Kraus representation](../../../../../../../kraus-representation.md) $\Lambda(X)=\sum_kA_kXA_k^\dagger$ gives

$$
F_e(\rho,\Lambda)
=\sum_k\left|
\langle\Psi_\rho|I\otimes A_k|\Psi_\rho\rangle
\right|^2.
$$

In a [Schmidt decomposition](../../../../../../../schmidt-decomposition.md) of the purification,

$$
\langle\Psi_\rho|I\otimes A_k|\Psi_\rho\rangle
=\sum_j\lambda_j\langle j|A_k|j\rangle
=\operatorname{Tr}(A_k\rho).
$$

Therefore

$$
\boxed{F_e(\rho,\Lambda)
=\sum_k|\operatorname{Tr}(A_k\rho)|^2}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
