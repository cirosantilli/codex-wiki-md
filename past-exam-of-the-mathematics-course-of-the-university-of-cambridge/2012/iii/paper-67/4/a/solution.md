<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $M=2^m$ and prepare $m$ control [qubits](../../../../../../qubit.md) in $|0\rangle^{\otimes m}$ and the target in the supplied [eigenstate](../../../../../../eigenstate.md) $|\psi\rangle$. Apply a [Hadamard gate](../../../../../../hadamard-gate.md) to every control [qubit](../../../../../../qubit.md). Let $k=\sum_{j=0}^{m-1}2^jk_j$ denote the integer encoded in that [quantum register](../../../../../../quantum-register.md).

For every $j$, apply a [controlled unitary gate](../../../../../../controlled-unitary-gate.md) $U^{2^j}$ with control $k_j$ and the same target. The [quantum phase kickback](../../../../../../phase-kickback.md) yields

$$
\frac1{\sqrt M}\sum_{k=0}^{M-1}|k\rangle U^k|\psi\rangle=\frac1{\sqrt M}\sum_{k=0}^{M-1}e^{2\pi ikx/M}|k\rangle\otimes|\psi\rangle=\operatorname{QFT}_M|x\rangle\otimes|\psi\rangle.
$$

Applying $\operatorname{QFT}_M^{-1}$ to the controls therefore produces $|x\rangle$ exactly. A [computational-basis measurement](../../../../../../quantum-measurement-in-the-computational-basis.md) returns $x$ with certainty, and the algorithm outputs

$$
\boxed{\phi=x/2^m.}
$$

This is [exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md); exactness uses the finite dyadic phase promise, not a rounding argument.

Only a [controlled-U gate](../../../../../../controlled-unitary-gate.md) is supplied as a primitive. Its $2^j$ repetitions implement controlled-$U^{2^j}$, so the total number of black-box uses is $\sum_{j=0}^{m-1}2^j=2^m-1$. Access to powers as unit-cost primitives would be a different [quantum query complexity](../../../../../../quantum-query-complexity.md) model. This distinction is the [cost of exact phase estimation on a dyadic spectrum](../../../../../../cost-of-exact-phase-estimation-on-a-dyadic-spectrum.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
