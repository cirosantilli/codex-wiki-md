<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $R=|\psi\rangle\langle\psi|$ and choose an [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|e_\mu\rangle\}$ of $\mathcal H_2$. The [reduced density matrix](../../../../../../reduced-density-matrix.md) on $S_1$ is the [partial trace](../../../../../../partial-trace.md)

$$
\boxed{\rho_1=\operatorname{Tr}_2R=\sum_\mu(I_1\otimes\langle e_\mu|)R(I_1\otimes|e_\mu\rangle).}
$$

Here $I_1$ is the identity on $\mathcal H_1$, and the bras and kets in the sum contract only the second tensor factor. Equivalently, if $|\psi\rangle=\sum_{a,\mu}c_{a\mu}|f_a\rangle\otimes|e_\mu\rangle$, then $(\rho_1)_{ab}=\sum_\mu c_{a\mu}c_{b\mu}^*$. The definition is independent of the chosen basis: it is characterized by $\operatorname{Tr}(M\rho_1)=\operatorname{Tr}[(M\otimes I_2)R]$ for every operator $M$ on $\mathcal H_1$.

The [generalized measurement postulate](../../../../../../generalized-measurement-postulate.md) takes $A_i$ to be operators on $\mathcal H_2$ satisfying $\sum_iA_i^\dagger A_i=I_2$. The [Born rule](../../../../../../born-rule.md) and the conditional state update give

$$
\boxed{p_i=\langle\psi|I_1\otimes A_i^\dagger A_i|\psi\rangle,\qquad |\psi_i\rangle=\frac{(I_1\otimes A_i)|\psi\rangle}{\sqrt{p_i}}\quad(p_i>0).}
$$

If the outcome is not supplied to $S_1$, the appropriate post-measurement [density matrix](../../../../../../density-matrix.md) is $R'=\sum_i(I_1\otimes A_i)R(I_1\otimes A_i^\dagger)$. For any local operator $M$, cyclicity of the full [trace](../../../../../../matrix-trace.md) gives

$$
\begin{aligned}
\operatorname{Tr}[(M\otimes I_2)R']
&=\sum_i\operatorname{Tr}[(M\otimes A_i^\dagger A_i)R]\\
&=\operatorname{Tr}[(M\otimes I_2)R].
\end{aligned}
$$

Since this holds for every $M$, $\boxed{\operatorname{Tr}_2R'=\rho_1}$. This is the [no-communication theorem](../../../../../../no-communication-theorem.md).

The invariance concerns the nonselective [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md). A conditional [reduced density matrix](../../../../../../reduced-density-matrix.md) $\rho_{1|i}=\operatorname{Tr}_2|\psi_i\rangle\langle\psi_i|$ can change, although $\sum_i p_i\rho_{1|i}=\rho_1$. For example, measuring one half of a [Bell pair](../../../../../../bell-pair.md) in the [computational basis](../../../../../../computational-basis.md) changes the other half conditionally to $|0\rangle$ or $|1\rangle$; before learning the outcome, its [density matrix](../../../../../../density-matrix.md) remains $I/2$. Thus distant [measurement in quantum measurements](../../../../../../quantum-measurement-split.md) cannot transmit a controllable signal without classical communication. This [quantum no-signalling](../../../../../../quantum-no-signalling.md) is compatible with [special relativity](../../../../../../special-relativity-split.md), even though some [entangled](../../../../../../entangled-state.md) states have correlations incompatible with a [local hidden-variable theory](../../../../../../local-hidden-variable-theory.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
