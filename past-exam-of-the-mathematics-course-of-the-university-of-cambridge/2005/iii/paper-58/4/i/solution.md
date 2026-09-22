<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [positive operator](../../../../../../positive-operator.md) $A$, the [spectral theorem](../../../../../../spectral-theorem.md) writes $A=\sum_j a_j|j\rangle\langle j|$ with $a_j\ge0$. Hence its unique [positive square root of an operator](../../../../../../positive-square-root-of-an-operator.md) is $\sqrt A=\sum_j\sqrt{a_j}|j\rangle\langle j|$. Conjugating this spectral decomposition shows $\sqrt{UAU^\dagger}=U\sqrt A U^\dagger$ for a [unitary operator](../../../../../../unitary-operator.md) $U$.

Let $\Delta=\rho_1-\rho_2$ and $\rho_i'=U\rho_iU^\dagger$. Then $\Delta'=U\Delta U^\dagger$ and $(\Delta')^\dagger\Delta'=U\Delta^\dagger\Delta U^\dagger$. The square-root covariance and the [cyclic property of the trace](../../../../../../cyclic-property-of-the-trace.md) give

$$
D(\rho_1',\rho_2')=\frac12\operatorname{Tr}\!\left(U\sqrt{\Delta^\dagger\Delta}\,U^\dagger\right)=\frac12\operatorname{Tr}\sqrt{\Delta^\dagger\Delta}=D(\rho_1,\rho_2).
$$

For the [quantum fidelity](../../../../../../fidelity-of-quantum-states.md), covariance first gives $(\rho_1')^{1/2}=U\rho_1^{1/2}U^\dagger$. Therefore

$$
(\rho_1')^{1/2}\rho_2'(\rho_1')^{1/2}=U\bigl(\rho_1^{1/2}\rho_2\rho_1^{1/2}\bigr)U^\dagger.
$$

Apply the same square-root identity and the [cyclic property of the trace](../../../../../../cyclic-property-of-the-trace.md) to obtain

$$
F(\rho_1',\rho_2')=\operatorname{Tr}\!\left(U\sqrt{\rho_1^{1/2}\rho_2\rho_1^{1/2}}\,U^\dagger\right)=F(\rho_1,\rho_2).
$$

Thus [unitary invariance of trace distance and fidelity](../../../../../../unitary-invariance-of-trace-distance-and-fidelity.md) gives

$$
\boxed{D(U\rho_1U^\dagger,U\rho_2U^\dagger)=D(\rho_1,\rho_2),\qquad F(U\rho_1U^\dagger,U\rho_2U^\dagger)=F(\rho_1,\rho_2).}
$$

The same $U$ acts on both [quantum states](../../../../../../quantum-state.md): these quantities depend on the relative distinguishability of the [quantum states](../../../../../../quantum-state.md), not on a choice of basis.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
