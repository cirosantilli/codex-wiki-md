<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the arbitrary initial [pure state](../../../../../../pure-state.md) as

$$
|\chi\rangle_{QR}=|0\rangle_Q|r_0\rangle_R+|1\rangle_Q|r_1\rangle_R,
\qquad\langle r_0|r_0\rangle+\langle r_1|r_1\rangle=1.
$$

The reference vectors need not be normalized or [orthogonal](../../../../../../orthogonal-vectors.md). By [linearity](../../../../../../linearity.md), the same [quantum teleportation](../../../../../../quantum-teleportation.md) calculation, with the [identity operator](../../../../../../identity-operator.md) on $R$, gives the post-gate [quantum state](../../../../../../quantum-state.md)

$$
\frac12\sum_{m,n=0}^1|mn\rangle_{QA}
\left[(X_B^nZ_B^m)\otimes I_R\right]
\left(|0\rangle_B|r_0\rangle_R+|1\rangle_B|r_1\rangle_R\right).
$$

Thus each outcome still has [probability](../../../../../../probability.md) $1/4$. Bob's [Pauli gate](../../../../../../pauli-gate.md) correction leaves the normalized joint [quantum state](../../../../../../quantum-state.md)

$$
\boxed{|\chi\rangle_{BR}=|0\rangle_B|r_0\rangle_R+|1\rangle_B|r_1\rangle_R.}
$$

All operations act trivially on $R$, so the result is independent of its holder or location. This establishes [teleportation as an identity channel on a reference](../../../../../../teleportation-as-an-identity-channel-on-a-reference.md), preserving [quantum entanglement](../../../../../../entangled-state.md) with the untouched reference. Since every corrected branch is the same, discarding the classical outcomes also leaves the required joint [density matrix](../../../../../../density-matrix-split.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
