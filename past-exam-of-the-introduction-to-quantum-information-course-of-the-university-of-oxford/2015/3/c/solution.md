<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize the second [qubit](../../../../qubit.md) as $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$. Since a [Pauli X gate](../../../../pauli-x-gate.md) changes $|-\rangle$ to $-|-\rangle$, the [Boolean quantum oracle](../../../../boolean-quantum-oracle.md) acts as

$$
U_f|x\rangle|-\rangle=(-1)^{f(x)}|x\rangle|-\rangle.
$$

This [quantum phase kickback](../../../../phase-kickback.md) leaves the second [qubit](../../../../qubit.md) uncorrelated with the first. Put $b=f(0)\oplus f(1)$: $b=0$ for a [constant function](../../../../constant-function.md) and $b=1$ for a [balanced Boolean function](../../../../balanced-boolean-function.md). Apart from the irrelevant [global phase](../../../../global-phase.md) $(-1)^{f(0)}$, the first [qubit](../../../../qubit.md) and environment reach

$$
\frac{|0\rangle|e_0\rangle+(-1)^b|1\rangle|e_1\rangle}{\sqrt2}.
$$

The population-preserving interaction commutes with the [quantum oracle](../../../../quantum-oracle.md) on this answer-register input, so its placement before or after the oracle, between the two [Hadamard gates](../../../../hadamard-gate.md), gives the same result. Substitute $\varphi=\pi b$ into [b](../b.md):

$$
\boxed{P(0\mid b)=\frac{1+(-1)^b v\cos\alpha}{2},\qquad
P(1\mid b)=\frac{1-(-1)^b v\cos\alpha}{2}.}
$$

The printed [Deutsch algorithm](../../../../deutsch-algorithm.md) uses the rule **zero means [constant function](../../../../constant-function.md); one means [balanced Boolean function](../../../../balanced-boolean-function.md)**. With that rule, the [Deutsch algorithm with pure dephasing](../../../../deutsch-algorithm-with-pure-dephasing.md) succeeds for either class with

$$
\boxed{P_{\rm correct}^{\rm printed}=\frac{1+v\cos\alpha}{2}.}
$$

For real nonnegative environment overlap this is $(1+v)/2$, ranging from certainty at $v=1$ to random guessing at $v=0$. For general complex overlap, a coherent shift can invert the printed answer: for example $v=1,\alpha=\pi$ makes the printed rule always wrong. If the overlap is known but the printed [quantum measurement](../../../../quantum-measurement-split.md) is retained, choose the better labeling of its outcomes; this gives

$$
\boxed{P_{\rm correct}^{\rm relabeled}=\frac{1+|v\cos\alpha|}{2}.}
$$

There is a further improvement if a known $\alpha$ can be compensated by the [phase gate](../../../../phase-gate.md) $P_{-\alpha}$ before the final [Hadamard gate](../../../../hadamard-gate.md). It removes the coherent shift without reversing any actual [quantum decoherence](../../../../quantum-decoherence.md), and yields

$$
\boxed{P_{\rm correct}^{\rm compensated}=\frac{1+v}{2}.}
$$

This is optimal when only the first [qubit](../../../../qubit.md) is accessible, with equal prior [probabilities](../../../../probability.md) for the two classes. Before the final [Hadamard gate](../../../../hadamard-gate.md), their [reduced density matrices](../../../../reduced-density-matrix.md) are

$$
\rho_b=\frac12\begin{pmatrix}1&(-1)^b\overline c\\(-1)^bc&1\end{pmatrix}.
$$

The difference $\rho_0-\rho_1$ has [eigenvalues](../../../../eigenvalue.md) $\pm v$, giving [trace distance](../../../../trace-distance.md) $v$. The [Holevo–Helstrom theorem](../../../../holevo-helstrom-theorem.md) therefore bounds the success [probability](../../../../probability.md) by $(1+v)/2$, exactly attained by the compensated procedure. A known phase shift and loss of coherence have different effects: at $v=0$ the two [density matrices](../../../../density-matrix-split.md) coincide and no measurement on the available [qubit](../../../../qubit.md) can reveal the answer.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
