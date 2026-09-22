<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The basic [one-bit teleportation](../../../../../../../one-bit-teleportation.md) primitive uses the input as [qubit](../../../../../../../qubit.md) 1 and a fresh $|+\rangle$ [quantum ancilla](../../../../../../../quantum-ancilla.md) as [qubit](../../../../../../../qubit.md) 2. Apply the [Controlled-Z gate](../../../../../../../controlled-z-gate.md) $E_{12}$ and measure [qubit](../../../../../../../qubit.md) 1 in the [equatorial qubit measurement](../../../../../../../equatorial-qubit-measurement.md) basis with angle $\alpha$. If $s\in\{0,1\}$ is the result, the normalized [post-measurement state](../../../../../../../post-measurement-state.md) on [qubit](../../../../../../../qubit.md) 2 is

$$
\boxed{X_2^sJ(\alpha)_2|\psi\rangle.}
$$

Both results have probability one half. For example, writing $|\psi\rangle=a|0\rangle+b|1\rangle$, the unnormalized branch is $(a|+\rangle+(-1)^se^{i\alpha}b|-\rangle)/\sqrt2=X^sJ(\alpha)|\psi\rangle/\sqrt2$. Thus $J(\alpha)$ is applied deterministically as a logical gate with known [Pauli frame](../../../../../../../pauli-frame.md) $X^s$; a permitted conditional [Pauli X gate](../../../../../../../pauli-x-gate.md) would remove this byproduct physically.

The literal resource restriction does not need an unstated direct [Pauli X gate](../../../../../../../pauli-x-gate.md). A [Pauli Z gate](../../../../../../../pauli-z-gate.md) can be enacted by applying $E$ to the data and a fixed $|1\rangle$ [quantum ancilla](../../../../../../../quantum-ancilla.md). Two consecutive angle-zero [one-bit teleportations](../../../../../../../one-bit-teleportation.md), with results $p,q$, map an arbitrary current state $|\chi\rangle$ to $X^qH X^pH|\chi\rangle=X^qZ^p|\chi\rangle$. Apply the available $Z^p$ to remove the latter factor, up to an irrelevant [global phase](../../../../../../../global-phase.md). This implements a heralded $X^q$: if $q=0$, the input is unchanged; if $q=1$, the required [Pauli X gate](../../../../../../../pauli-x-gate.md) has been applied.

If the original result is $s=1$ and a physically corrected output is required, repeat this [heralded Pauli X correction using controlled-Z and measurements](../../../../../../../heralded-pauli-x-correction-using-controlled-z-and-measurements.md) until $q=1$. Each attempt succeeds with probability one half independent of the input, so it terminates with probability one, using two attempts on average. Only $E$, fixed ancillary [quantum states](../../../../../../../quantum-state.md) and single-[qubit](../../../../../../../qubit.md) [measurement in quantum measurements](../../../../../../../quantum-measurement-split.md) are used. This exact physical correction has no finite worst-case measurement bound; the standard finite deterministic realization is the logical [Pauli frame](../../../../../../../pauli-frame.md) version, which suffices for the later output-simulation parts.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
