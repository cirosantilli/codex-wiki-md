<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Kraus operators](../../../../../kraus-operator.md) of the [generalized measurement postulate](../../../../../generalized-measurement-postulate.md) must obey

$$
\boxed{\sum_i A_i^\dagger A_i=I.}
$$

For a normalized [pure state](../../../../../pure-state.md), the [Born rule](../../../../../born-rule.md) gives the outcome probability and the normalized conditional state:

$$
\boxed{p_i=\langle\psi|A_i^\dagger A_i|\psi\rangle=\lVert A_i|\psi\rangle\rVert^2,\qquad|\psi_i\rangle=\frac{A_i|\psi\rangle}{\sqrt{p_i}}\quad(p_i>0).}
$$

Here the dagger denotes the [Hermitian conjugate](../../../../../hermitian-conjugation.md). Completeness ensures $\sum_i p_i=1$. An outcome with $p_i=0$ never occurs for that input, so no conditional state is required there. The positive operators $E_i=A_i^\dagger A_i$ form a [POVM](../../../../../positive-operator-valued-measure.md), but the actual operators $A_i$ also specify the post-measurement states.

Let $\rho_{12}=|\Psi\rangle\langle\Psi|$ be the initial joint [density operator](../../../../../density-matrix.md), and $\rho_2=\operatorname{Tr}_1\rho_{12}$ its [reduced density matrix](../../../../../reduced-density-matrix.md) on the accessible subsystem. If the first experimenter performs the measurement, the conditional joint state for outcome $i$ is $(A_i\otimes I)\rho_{12}(A_i^\dagger\otimes I)/p_i$. The second experimenter does not know that outcome. The relevant [nonselective quantum measurement](../../../../../nonselective-quantum-measurement.md) state is therefore the probability-weighted average

$$
\rho'_{12}=\sum_i(A_i\otimes I)\rho_{12}(A_i^\dagger\otimes I).
$$

To compare the accessible states, take any operator $B$ on the second subsystem. Cyclicity of the [trace](../../../../../matrix-trace.md) and the fact that operators on different tensor factors commute give

$$
\begin{aligned}
\operatorname{Tr}[(I\otimes B)\rho'_{12}]&=\sum_i\operatorname{Tr}[(A_i^\dagger A_i\otimes B)\rho_{12}]\\
&=\operatorname{Tr}[(I\otimes B)\rho_{12}].
\end{aligned}
$$

By the defining property of the [partial trace](../../../../../partial-trace.md), this says $\operatorname{Tr}(B\rho'_2)=\operatorname{Tr}(B\rho_2)$ for every $B$. Matrix units, or arbitrary Hermitian test operators, distinguish any two different [density matrices](../../../../../density-matrix.md), so

$$
\boxed{\rho'_2=\rho_2.}
$$

This proves [remote state invariance under a local trace-preserving operation](../../../../../remote-state-invariance-under-a-local-trace-preserving-operation.md) directly from completeness.

In particular, if the accessible experiment has [POVM](../../../../../positive-operator-valued-measure.md) elements $F_k$, its probabilities are $\operatorname{Tr}(F_k\rho'_2)=\operatorname{Tr}(F_k\rho_2)$ whether the distant measurement happens or not. Attaching an independent local ancilla, evolving locally, or performing a sequence of local measurements cannot help: these operations act on the identical input [density operator](../../../../../density-matrix.md) and therefore give identical outcome distributions. **No experiment confined to the second subsystem can distinguish whether the unannounced measurement occurred.** This is a derivation of the [no-communication theorem](../../../../../no-communication-theorem.md), not an appeal to a signalling postulate.

The qualification is that the outcome is not communicated. A [selective quantum measurement](../../../../../selective-quantum-measurement.md) can give different conditional remote states, as happens when measuring one half of a [Bell state](../../../../../bell-state-split.md); their probability-weighted average is still $\rho_2$. An observer supplied with the distant outcome has extra classical information and is no longer restricted to the unannounced local experiment considered here.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
