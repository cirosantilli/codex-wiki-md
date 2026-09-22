<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the [Bernstein-Vazirani algorithm](../../../../../bernstein-vazirani-algorithm.md): initialize n [qubits](../../../../../qubit.md) in $|0^n\rangle$, apply $H^{\otimes n}$, query the supplied [phase oracle](../../../../../phase-oracle.md) once, apply $H^{\otimes n}$ again, and measure all n computational bits. Immediately after the query the state is

$$
\frac1{\sqrt{2^n}}\sum_x(-1)^{a\cdot x}|x\rangle,
$$

where the dot product in the exponent is taken modulo two. The [Walsh-Hadamard transform](../../../../../walsh-hadamard-transform.md) gives amplitude

$$
\begin{aligned}
\langle y|H^{\otimes n}O_fH^{\otimes n}|0^n\rangle
&=\frac1{2^n}\sum_{x\in\{0,1\}^n}(-1)^{(a\oplus y)\cdot x}\\
&=\prod_{j=1}^n\frac{1+(-1)^{a_j\oplus y_j}}2.
\end{aligned}
$$

Every factor is one if $y_j=a_j$ and zero otherwise. Thus the final state is **exactly $|a\rangle$**, and the measurement outputs a with certainty after **one oracle query**. This is the character cancellation behind [Bernstein-Vazirani phase kickback](../../../../../bernstein-vazirani-phase-kickback.md); because access here is already to the reduced [phase oracle](../../../../../phase-oracle.md), no extra target ancilla or conversion from a bit-flip oracle is required.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
