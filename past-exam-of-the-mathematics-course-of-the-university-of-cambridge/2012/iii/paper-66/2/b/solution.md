<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the arbitrary joint [pure state](../../../../../../pure-state.md) of the input $A$ and an external reference $R$ as

$$
|\Omega\rangle_{AR}=|0\rangle_A|r_0\rangle_R+|1\rangle_A|r_1\rangle_R,
\qquad \langle r_0|r_0\rangle+\langle r_1|r_1\rangle=1.
$$

The reference vectors need not be normalized or orthogonal. Share $|\Phi^+\rangle_{aB}$. Label Alice's [Bell states](../../../../../../bell-state-split.md) by

$$
|\beta_{rs}\rangle_{Aa}
=\frac1{\sqrt2}\sum_{j=0}^1(-1)^{rj}|j\rangle_A|j\oplus s\rangle_a,
\qquad r,s\in\{0,1\}.
$$

Projecting onto this [Bell basis](../../../../../../bell-basis.md) gives the unnormalized state

$$
{}_{Aa}\langle\beta_{rs}|\left(|\Omega\rangle_{AR}|\Phi^+\rangle_{aB}\right)
=\frac12(X_B^sZ_B^r\otimes I_R)|\Omega\rangle_{BR}.
$$

Each outcome has probability $1/4$. Alice sends $(r,s)$ and Bob applies **$Z_B^rX_B^s$**, reversing the two [Pauli gates](../../../../../../pauli-gate.md). The final state is exactly $|\Omega\rangle_{BR}$ for every outcome. In particular all input [entanglement](../../../../../../entangled-state.md) and other correlations with $R$ now belong to $B$, while the reference marginal is unchanged. This is [teleportation as an identity channel on a reference](../../../../../../teleportation-as-an-identity-channel-on-a-reference.md).

Conditioned on the record, Alice's two measured carriers are in $|\beta_{rs}\rangle$ and factor from $BR$. Thus $A$ no longer retains its original correlations with $R$. There is no second copy, even when the teleported [qubit](../../../../../../qubit.md) was initially [entangled](../../../../../../entangled-state.md) with a larger system.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
