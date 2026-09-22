<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A deterministic quantum operation here is a [CPTP map](../../../../../../quantum-channel.md). By [Stinespring dilation](../../../../../../stinespring-dilation.md), there is an [isometry](../../../../../../isometry.md) $V:B\to B'E$ with $\Lambda(\tau)=\operatorname{Tr}_E(V\tau V^\dagger)$. Let $\omega_{AB'E}=(I\otimes V)\rho_{AB}(I\otimes V^\dagger)$. An [isometry](../../../../../../isometry.md) preserves all nonzero eigenvalues, so

$$
I(A:B'E)_\omega=I(A:B)_\rho.
$$

The [quantum mutual information](../../../../../../quantum-mutual-information.md) is $I(A:B)=S(A)+S(B)-S(AB)$. The difference after discarding the environment is

$$
\begin{aligned}
I(A:B'E)_\omega-I(A:B')_\omega
&=S(AB')+S(B'E)-S(B')-S(AB'E)\\
&=I(A:E\mid B')_\omega\geq0,
\end{aligned}
$$

where the last inequality is [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md), in the form $S(AB')+S(B'E)\geq S(B')+S(AB'E)$. Thus [data processing for quantum mutual information](../../../../../../data-processing-for-quantum-mutual-information.md) gives

$$
\boxed{I(A':B')\leq I(A:B).}
$$

Subsystem $A$ is unchanged; its prime simply labels the output. Keeping the environment would preserve the mutual information, while tracing it out cannot increase it.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
