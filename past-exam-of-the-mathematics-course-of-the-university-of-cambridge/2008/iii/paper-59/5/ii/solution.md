<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a bipartite state $\rho_{AB}$, let a [local operation](../../../../../../local-quantum-operation.md) on A have [Kraus operators](../../../../../../kraus-operator.md) $M_\alpha$ satisfying $\sum_\alpha M_\alpha^\dagger M_\alpha=I$. Without selecting its outcome, the state becomes

$$
\rho'_{AB}=\sum_\alpha(M_\alpha\otimes I)\rho_{AB}(M_\alpha^\dagger\otimes I).
$$

For every remote [observable](../../../../../../observable.md) $B$, cyclicity of the trace gives

$$
\operatorname{tr}[\rho'_{AB}(I\otimes B)]=\operatorname{tr}\left[\rho_{AB}\left(\sum_\alpha M_\alpha^\dagger M_\alpha\otimes B\right)\right]=\operatorname{tr}[\rho_{AB}(I\otimes B)].
$$

Therefore the remote [partial trace](../../../../../../partial-trace.md) is unchanged:

$$
\boxed{\rho'_B=\rho_B.}
$$

This proves [quantum no-signalling](../../../../../../quantum-no-signalling.md) for local trace-preserving [quantum channels](../../../../../../quantum-channel.md), including choices between different such operations. It makes no assumption that $\rho_{AB}$ is separable.

Conditioning on one outcome instead uses an unnormalized state with only that outcome's [Kraus operators](../../../../../../kraus-operator.md) and then divides by its probability. Its remote conditional state can change, yielding quantum steering. However, the outcome cannot be selected deterministically by choosing the measurement setting, and the remote observer needs an ordinary message identifying the selected ensemble. Ignoring the outcome restores the unchanged marginal. [No-signalling](../../../../../../quantum-no-signalling.md) thus concerns operationally accessible unconditional statistics, not equality of every conditional probability.

The proof presupposes that the intervention is genuinely confined to A and is trace-preserving when outcomes are ignored. A nonlocal operation or setting-dependent postselection does not meet those premises. In field theory local algebras need not come with a simple finite-dimensional tensor factorization; the corresponding statement is expressed using commuting local algebras and [local operations](../../../../../../local-quantum-operation.md), as below.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
