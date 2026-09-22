<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Embed the given purifications into a common reference [Hilbert space](../../../../../../hilbert-space-split.md) $R$, enlarging it if necessary, and add a flag register $X$ with [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|x\rangle\}$. A [flagged purification of a quantum ensemble](../../../../../../flagged-purification-of-a-quantum-ensemble.md) is

$$
\boxed{|\Psi\rangle_{ARX}=\sum_x\sqrt{p_x}\,|\psi_{\rho_x}\rangle_{AR}\otimes|x\rangle_X.}
$$

Orthogonality of the flags gives $\langle\Psi|\Psi\rangle=\sum_xp_x=1$. Moreover,

$$
\operatorname{Tr}_{RX}|\Psi\rangle\langle\Psi|
=\sum_{x,z}\sqrt{p_xp_z}\,\langle z|x\rangle\operatorname{Tr}_R|\psi_{\rho_x}\rangle\langle\psi_{\rho_z}|
=\sum_xp_x\rho_x=\rho.
$$

Thus it is a [purification of a density operator](../../../../../../purification-of-a-density-operator.md). The extra flag is essential: simply superposing the purifications without orthogonal labels would generally leave unwanted cross terms.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
