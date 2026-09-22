# Deterministic reduction of maximally entangled Schmidt rank

↑ **Parent:** [Local operations and classical communication](local-operations-and-classical-communication.md)

Let $|\Phi_d\rangle=d^{-1/2}\sum_{j=0}^{d-1}|j,j\rangle$ and $1\leq m\leq d$. It can be converted deterministically by [LOCC](local-operations-and-classical-communication.md) to $|\Phi_m\rangle$. For each $m$-element subset $S$ of the local basis labels, let $\Pi_S$ be its projector and let Alice's [Kraus operator](kraus-operator.md) be $K_S=\Pi_S/\sqrt{\binom{d-1}{m-1}}$. Every label occurs in $\binom{d-1}{m-1}$ subsets, so $\sum_SK_S^\dagger K_S=I$. Each outcome has [probability](probability.md) $m/[d\binom{d-1}{m-1}]=1/\binom dm$ and leaves the [maximally entangled state](maximally-entangled-state.md) $m^{-1/2}\sum_{j\in S}|j,j\rangle$. Alice reports $S$, and both parties relabel these $m$ basis states to $0,\ldots,m-1$ by [local unitary operations](local-unitary-operation.md).

For $d=6$, $m=4$, only three outcomes are needed: partition the six labels into disjoint pairs $T_0,T_1,T_2$ and use $K_r=(I-\Pi_{T_r})/\sqrt2$. Each label is retained twice, proving completeness, and each outcome has [probability](probability.md) $1/3$. Every branch leaves four equal [Schmidt coefficients](schmidt-coefficient.md), hence two independent [Bell pairs](bell-pair.md) after binary relabelling.

## ↑ Ancestors (6)

1. [Local operations and classical communication](local-operations-and-classical-communication.md)
2. [Bell state](bell-state-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/3/solution.md)
