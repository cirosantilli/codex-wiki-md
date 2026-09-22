<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Take a [Stinespring dilation](../../../../../../stinespring-dilation.md) $V:B\longrightarrow B'E$ of the local [quantum channel](../../../../../../quantum-channel.md) and define $\tau_{AB'E}=(I_A\otimes V)\rho_{AB}(I_A\otimes V^\dagger)$. Tracing out $E$ gives the prescribed output, with $A'=A$. An isometry preserves the nonzero eigenvalues of a [density operator](../../../../../../density-matrix.md); therefore $S(B'E)_\tau=S(B)_\rho$, $S(AB'E)_\tau=S(AB)_\rho$, and $S(A)_\tau=S(A)_\rho$.

Consequently $I(A:B'E)_\tau=I(A:B)_\rho$. The loss of [quantum mutual information](../../../../../../quantum-mutual-information.md) is

$$
\begin{aligned}
I(A:B)_\rho-I(A':B')_\sigma
&=I(A:B'E)_\tau-I(A:B')_\tau\\
&=S(AB')_\tau+S(B'E)_\tau-S(B')_\tau-S(AB'E)_\tau\\
&=I(A:E\mid B')_\tau\geq0.
\end{aligned}
$$

The last inequality is [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md), or nonnegativity of [quantum conditional mutual information](../../../../../../quantum-conditional-mutual-information.md). Hence

$$
\boxed{I(A':B')_\sigma\leq I(A:B)_\rho.}
$$

This [mutual-information loss as conditional mutual information](../../../../../../mutual-information-loss-as-conditional-mutual-information.md) shows exactly which correlations are discarded into the environment. No purity assumption on the original state is needed.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
