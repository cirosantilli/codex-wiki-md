<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the [quantum channel](../../../../../../quantum-channel.md) send $B$ to $B'$. From its [Kraus representation](../../../../../../kraus-representation.md), choose a [Stinespring representation](../../../../../../stinespring-representation-of-a-completely-positive-map.md) $V:B\to B'E$ and form

$$
\sigma_{AB'E}=(I_A\otimes V)\rho_{AB}(I_A\otimes V^\dagger).
$$

The channel output is $\sigma_{AB'}=\operatorname{Tr}_E\sigma_{AB'E}$. Isometric invariance of [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) gives

$$
S(B'E)_\sigma=S(B)_\rho,\quad S(AB'E)_\sigma=S(AB)_\rho,\quad S(A)_\sigma=S(A)_\rho.
$$

Therefore the [quantum mutual information](../../../../../../quantum-mutual-information.md) satisfies $I(A:B)_\rho=I(A:B'E)_\sigma$. Expanding its loss after discarding the environment gives

$$
\begin{aligned}
I(A:B)_\rho-I(A:B')_\sigma
&=I(A:B'E)_\sigma-I(A:B')_\sigma\\
&=S(AB')_\sigma+S(B'E)_\sigma-S(B')_\sigma-S(AB'E)_\sigma.
\end{aligned}
$$

The final expression is the [quantum conditional mutual information](../../../../../../quantum-conditional-mutual-information.md) $I(A:E\mid B')$. The [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md) states exactly that it is nonnegative. Hence

$$
\boxed{I(A:B')\leq I(A:B).}
$$

This proves [data processing for quantum mutual information](../../../../../../data-processing-for-quantum-mutual-information.md) for any mixed input and any local [quantum channel](../../../../../../quantum-channel.md), not just the atomic channel in earlier parts. The correlations lost are exactly the conditional correlations with the discarded environment.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
