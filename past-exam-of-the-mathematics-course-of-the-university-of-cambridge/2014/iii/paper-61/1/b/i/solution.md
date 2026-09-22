<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Prepare an additional [qubit](../../../../../../../qubit.md) in $|{-}\rangle=(|0\rangle-|1\rangle)/\sqrt2$ by applying $X$ and then the [Hadamard gate](../../../../../../../hadamard-gate.md) to $|0\rangle$. Apply $H^{\otimes n}$ to the data register. The [Boolean quantum oracle](../../../../../../../boolean-quantum-oracle.md) then produces [quantum phase kickback](../../../../../../../phase-kickback.md):

$$
\frac1{\sqrt{2^n}}\sum_x|x\rangle|{-}\rangle
\stackrel{U_f}{\longmapsto}
\frac1{\sqrt{2^n}}\sum_x(-1)^{a\cdot x}|x\rangle|{-}\rangle.
$$

A final [Walsh-Hadamard transform](../../../../../../../walsh-hadamard-transform.md) gives an amplitude for $z$ equal to

$$
\frac1{2^n}\sum_x(-1)^{(a\oplus z)\cdot x}=\delta_{z,a}.
$$

To see this identity, the sum factors over the bits; any position at which $a$ and $z$ differ contributes $1-1=0$. This is [Bernstein-Vazirani phase kickback](../../../../../../../bernstein-vazirani-phase-kickback.md), and its output is

$$
\boxed{|a\rangle|{-}\rangle}.
$$

There is exactly one oracle query, $O(n)$ fixed [quantum gates](../../../../../../../quantum-logic-gate.md), and no probabilistic intermediate step. The [ancilla qubit](../../../../../../../ancilla-qubit.md) can be left in $|A\rangle=|{-}\rangle$ or reset to $|0\rangle$ using its known inverse preparation. The construction includes the case $a=0$.

## ↑ Ancestors (12)

1. [I](../i.md)
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
