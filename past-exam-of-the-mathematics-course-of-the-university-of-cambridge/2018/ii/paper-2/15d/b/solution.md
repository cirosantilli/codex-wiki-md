<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Quantum no-signalling](../../../../../../quantum-no-signalling.md) says that, without communicating a measurement outcome, any local trace-preserving operation performed on subsystem $A$ leaves all outcome probabilities for measurements on subsystem $B$ unchanged; equivalently, it leaves the [reduced density matrix](../../../../../../reduced-density-matrix.md) $\rho_B$ unchanged.

The two Bell states are orthogonal. Applying the inverse Bell-state preparation circuit, namely a [Controlled-NOT gate](../../../../../../controlled-not-gate.md) from $A$ to $B$ followed by a [Hadamard gate](../../../../../../hadamard-gate.md) on $A$, gives

$$
|\phi^+\rangle\longmapsto|00\rangle,
\qquad
|\phi^-\rangle\longmapsto|10\rangle.
$$

A computational-basis measurement therefore distinguishes them perfectly, so

$$
\boxed{P_{\rm err}^{AB}=0.}
$$

If only $B$ is accessible, however,

$$
\operatorname{tr}_A|\phi^+\rangle\langle\phi^+|
=\operatorname{tr}_A|\phi^-\rangle\langle\phi^-|
=\frac I2.
$$

Every measurement on $B$ consequently has the same outcome distribution under both hypotheses. With equal prior probabilities no information is available, and

$$
\boxed{P_{\rm err}^{B}=\frac12,}
$$

the error probability of a random guess.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
