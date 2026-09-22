# Target no-signalling in a common-control unitary

↑ **Parent:** [Quantum no-signalling](quantum-no-signalling.md)

Let $U=\sum_b U_b^A\otimes|b\rangle\langle b|_B\otimes V_b^C$, where the conditional target operators are unitary. For product input $\rho_A\otimes\rho_B\otimes\rho_C$,

$$
\rho_C'=\sum_b\langle b|\rho_B|b\rangle V_b\rho_CV_b^\dagger.
$$

Tracing over $B$ removes cross terms with unequal control labels. Tracing over $A$ leaves $\operatorname{Tr}(U_b\rho_AU_b^\dagger)=1$, proving the formula and its independence of $\rho_A$. Exchanging $A$ and $C$ proves the corresponding reverse independence. Thus the two targets cannot signal to each other through this fixed common-control interaction, despite [phase kickback](phase-kickback.md) allowing a target to affect its control.

Two [controlled-NOT gates](controlled-not-gate.md) with a common control and distinct targets are an example. They commute; their chronological order can be exchanged, giving an equivalent causal proof. Intervening control rotations or additional interactions can change the conclusion.

## ↑ Ancestors (5)

1. [Quantum no-signalling](quantum-no-signalling.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/quantum-information/1/c/iv/solution.md)
