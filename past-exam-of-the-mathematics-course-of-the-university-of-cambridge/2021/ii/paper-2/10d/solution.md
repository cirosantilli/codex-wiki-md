<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

Apply a [Hadamard gate](../../../../../hadamard-gate.md) to every qubit. The amplitude of $|0^n\rangle$ becomes

$$
\langle0^n|H^{\otimes n}|\xi\rangle
=\frac1{2^n}\sum_{x\in\mathcal B_n}(-1)^{f(x)}.
$$

It equals $1$ in case (I) and $0$ in case (II). A [computational-basis measurement](../../../../../quantum-measurement-in-the-computational-basis.md) therefore returns $0^n$ with certainty in case (I) and never returns it in case (II). This is the [Deutsch-Jozsa algorithm](../../../../../deutsch-jozsa-algorithm.md).

For the distributed problem, Alice prepares

$$
|\xi_A\rangle=2^{-n/2}\sum_x(-1)^{f_A(x)}|x\rangle
$$

using one query to her [quantum oracle](../../../../../boolean-quantum-oracle.md), and sends these $n$ qubits to Bob. Bob applies his phase oracle, producing

$$
2^{-n/2}\sum_x(-1)^{f_A(x)\oplus f_B(x)}|x\rangle.
$$

The function $h=f_A\oplus f_B$ is constant zero in case (1) and balanced in case (2). Bob applies $H^{\otimes n}$ and measures as above: outcome $0^n$ identifies case (1), while every other outcome identifies case (2), with certainty.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
