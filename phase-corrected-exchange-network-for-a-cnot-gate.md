# Phase-corrected exchange network for a CNOT gate

↑ **Parent:** [Exchange-pulse CNOT synthesis](exchange-pulse-cnot-synthesis.md)

With $S=P_++iP_-$ the conventional [square root of the SWAP gate](square-root-of-the-swap-gate.md), $P=\operatorname{diag}(1,i)$ the [S gate](s-gate.md), and operators acting rightmost first, $SZ_1S=\operatorname{diag}(1,i,-i,-1)$. Therefore $H_2SZ_1SP_2H_2=|0\rangle\langle0|\otimes X-i|1\rangle\langle1|\otimes I$. Appending $X_2$ changes the zero-controlled flip into a one-controlled flip, and $P_1$ removes the control-dependent phase. This proves the displayed exact [CNOT gate](controlled-not-gate.md) identity. Both the exchange branch and the [phase gate](phase-gate.md) square-root convention matter; changing either requires recalculating the correction.

## ↑ Ancestors (9)

1. [Exchange-pulse CNOT synthesis](exchange-pulse-cnot-synthesis.md)
2. [Square root of the SWAP gate](square-root-of-the-swap-gate.md)
3. [SWAP gate](swap-gate.md)
4. [Controlled-NOT gate](controlled-not-gate.md)
5. [Controlled unitary gate](controlled-unitary-gate.md)
6. [Quantum theory](quantum-theory-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2008/8/3/solution.md)
