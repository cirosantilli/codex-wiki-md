<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [J gate](../../../../../../../j-gate-in-measurement-based-quantum-computation.md) is $J(\alpha)=HP(\alpha)$, with $P(\alpha)=\operatorname{diag}(1,e^{i\alpha})$. Prepare a fresh [qubit](../../../../../../../qubit.md) in $|+\rangle$ and apply the [Controlled-Z gate](../../../../../../../controlled-z-gate.md) $E$ between it and the input $|\psi\rangle=u|0\rangle+v|1\rangle$. The resulting state is

$$
u|0\rangle|+\rangle+v|1\rangle|-\rangle.
$$

Measure the input in the [equatorial qubit measurement](../../../../../../../equatorial-qubit-measurement.md) basis $|\alpha_s\rangle=(|0\rangle+(-1)^se^{-i\alpha}|1\rangle)/\sqrt2$. The unnormalized output is

$$
\frac1{\sqrt2}\left(u|+\rangle+(-1)^se^{i\alpha}v|-\rangle\right)
=\frac1{\sqrt2}X^sJ(\alpha)|\psi\rangle.
$$

Each outcome has probability $1/2$. Thus [one-bit teleportation](../../../../../../../one-bit-teleportation.md) realizes

$$
\boxed{|\psi\rangle\longmapsto X^sJ(\alpha)|\psi\rangle}
$$

on the new [qubit](../../../../../../../qubit.md). Apply the known [Pauli X gate](../../../../../../../pauli-x-gate.md) correction $X^s$ for the literal $J(\alpha)$ output, or keep the correction in a [Pauli frame](../../../../../../../pauli-frame.md) and adapt later measurements. The old [qubit](../../../../../../../qubit.md) is measured, so this is not cloning the input.

Direct multiplication of the given matrices gives $J(\alpha)X^s=e^{+is\alpha}Z^sJ((-1)^s\alpha)$. The displayed negative exponent in the supplied relation has the wrong sign for exact matrix equality. The discrepancy is only a [global phase](../../../../../../../global-phase.md) in a fixed measurement branch, so it does not change this measurement implementation or its outcome probabilities. The positive-sign identity is used when tracking exact matrices.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 61](../../../../paper-61-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
