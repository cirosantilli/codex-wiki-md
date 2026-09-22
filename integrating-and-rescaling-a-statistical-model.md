# Integrating and rescaling a statistical model

↑ **Parent:** [Renormalization group](renormalization-group.md)

Use a dimensionless [statistical Hamiltonian](statistical-hamiltonian.md) $\mathcal H=H/(k_BT)$, so that the [partition function](canonical-partition-function.md) is $Z=\sum_s e^{-\mathcal H(s)}$. Choose a [normalized blocking kernel](normalized-blocking-kernel.md) $B(S\mid s)$ with $\sum_S B(S\mid s)=1$. For the majority example it is one when every block has its prescribed majority, and zero otherwise. Define the coarse [statistical Hamiltonian](statistical-hamiltonian.md) by the displayed sum. Then an elementary interchange of finite sums proves

$$
Z'=\sum_S e^{-\mathcal H'(S)}=\sum_s e^{-\mathcal H(s)}\sum_S B(S\mid s)=Z.
$$

The probability of a retained pattern is therefore its original marginal probability. For any observable $A(S)$ of the retained variables,

$$
\langle A\rangle'=\frac1Z\sum_s e^{-\mathcal H(s)}\sum_S B(S\mid s)A(S).
$$

This is the sense in which elimination preserves predictions for retained information. It does not reconstruct every microscopic observable from a block sign.

Next express positions in units of the enlarged spacing: $x'=x/b$, where $b>1$. In a continuum version, rescale the retained [scalar field](scalar-field.md) as well to restore a chosen [gradient energy](gradient-energy.md) coefficient; any change in the integration measure contributes to the field-independent term. The result is a new set of dimensionless couplings. Repeating the procedure defines a [renormalization-group flow](renormalization-group-flow.md). Additional interactions and the additive constant generally appear, even if the starting [statistical Hamiltonian](statistical-hamiltonian.md) was simple. Keeping only a few terms is an approximation; the equality of [partition functions](canonical-partition-function.md) above applies to the complete coarse weight. See also the [Wilsonian coarse-grained statistical Hamiltonian](wilsonian-coarse-grained-statistical-hamiltonian.md) for integration over fast [Fourier modes](fourier-mode.md).

## ↑ Ancestors (6)

1. [Renormalization group](renormalization-group.md)
2. [Critical phenomenon](critical-phenomenon-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
