<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

Without Alice's operation, Bob obtains outcome $b$ with probability

$$
p(b)=\langle\psi|I_A\otimes|b\rangle\langle b|\psi\rangle.
$$

If Alice applies $U$ and then measures, but her outcome is not communicated, Bob's probability is

$$
\begin{aligned}
p'(b)
&=\sum_a\langle\psi|
U^\dagger\Pi_aU\otimes|b\rangle\langle b|\psi\rangle\\
&=\langle\psi|I_A\otimes|b\rangle\langle b|\psi\rangle=p(b),
\end{aligned}
$$

because $\sum_a\Pi_a=I_A$. Equivalently, a trace-preserving local operation leaves Bob's [reduced density matrix](../../../../../reduced-density-matrix.md) unchanged. This is the [no-communication theorem](../../../../../quantum-no-signalling.md): local operations cannot signal without communication of their outcomes.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
