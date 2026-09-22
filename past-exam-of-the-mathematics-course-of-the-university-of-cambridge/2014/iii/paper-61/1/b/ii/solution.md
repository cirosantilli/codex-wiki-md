<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The linear decoding must be done coherently, so its output is available inside the next [Boolean quantum oracle](../../../../../../../boolean-quantum-oracle.md) call. Use registers $Z,X$ of $n$ [qubits](../../../../../../../qubit.md) and a shared phase [ancilla qubit](../../../../../../../ancilla-qubit.md) in $|{-}\rangle$. Define the [Bernstein-Vazirani decoding controlled by a quantum register](../../../../../../../bernstein-vazirani-decoding-controlled-by-a-quantum-register.md)

$$
W_g=(H_Z^{\otimes n}\otimes I_X)\,U_g\,(H_Z^{\otimes n}\otimes I_X).
$$

The [ancilla qubit](../../../../../../../ancilla-qubit.md) is implicit. For every computational index $x$, the [Walsh-Hadamard transform](../../../../../../../walsh-hadamard-transform.md) calculation gives

$$
W_g|z\rangle_Z|x\rangle_X|{-}\rangle
=|z\oplus a_x\rangle_Z|x\rangle_X|{-}\rangle.
$$

In particular $W_g^2=I$ on these states. Initialize $Z$ to $|0\rangle$ and $X$ to $H^{\otimes n}|0\rangle$. The three query stages are

$$
\frac1{\sqrt{2^n}}\sum_x|0\rangle|x\rangle|{-}\rangle
\stackrel{W_g}{\longmapsto}
\frac1{\sqrt{2^n}}\sum_x|a_x\rangle|x\rangle|{-}\rangle
\stackrel{U_f}{\longmapsto}
\frac1{\sqrt{2^n}}\sum_x(-1)^{a\cdot x}|a_x\rangle|x\rangle|{-}\rangle
\stackrel{W_g}{\longmapsto}
|0\rangle\frac1{\sqrt{2^n}}\sum_x(-1)^{a\cdot x}|x\rangle|{-}\rangle.
$$

The middle equality uses the matching index $z=a_x$, not a classical guess of that string. The second $W_g$ performs [uncomputation](../../../../../../../uncomputation.md), removing the hidden-string register without losing its phase on $X$. Apply $H^{\otimes n}$ to $X$ to obtain

$$
\boxed{|0\rangle_Z|a\rangle_X|{-}\rangle}.
$$

This requires precisely two queries to $U_g$ and one to $U_f$, and only $O(n)$ additional fixed [quantum gates](../../../../../../../quantum-logic-gate.md). No measurement of $a_x$ is made: such a measurement would spoil the required coherence. Preparing all registers and the phase [ancilla qubit](../../../../../../../ancilla-qubit.md) uses only the initially available zero states.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 61](../../../../paper-61-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
